Il contenuto prevede uno smart contract denominato Windowshadow, scritto in solidity, importando librerie da openzeppelin. 
È utilizzato per la creazione di un token ERC-1155 che gestisce asset digitali, quindi token fungibili e token non fungiili.

All’interno del contratto vi è lo strumento Ownable che permette di assegnare un proprietario al contratto.

Al suo interno sono presenti 3 assets, il nome del set di Assets è "My Assets":
•	Diamante, al quale è stato attribuito ID 1; è previsto un mint iniziale di 100 unità.
•	Maniglia, alla quale è stato attribuito ID 2; è previsto un mint iniziale di 1 unità.
•	Vetro, al quale è stato attribuito ID 3; è previsto un mint iniziale di 1 unità.

Il codice contiene minting automatico, quindi al momento del deployment, gli assets saranno mintanti nell’address del proprietario.
Solo il proprietario può richiamare la funzione di minting.
Il deployment Crea il contratto e assegna i token iniziali all'owner, nonché proprietario.  
L’Owner (il proprietario) può cambiare l’URI dei metadati, creare nuovi token per account e mintare più token contemporanemente, come avviene in fase di deployment.
	
Il metadata URI è impostato per prendere i dati da Pinata IPFS. Sottostante, i relativi link:
•	File json  = https://emerald-imaginative-spoonbill-973.mypinata.cloud/ipfs/bafybeib5pxmcdxjyoifexaameij3dyisbw4gikbv2b4nvvrhhqg6mgk7nu/

•	Immagine Diamante= https://emerald-imaginative-spoonbill-973.mypinata.cloud/ipfs/bafybeifmehw7ebfkwm4jedaf34lhyswkfamxefkbnvqxryxcdcnvbozc7u/Diamante.png

•	Immagine Maniglia= https://emerald-imaginative-spoonbill-973.mypinata.cloud/ipfs/bafybeifmehw7ebfkwm4jedaf34lhyswkfamxefkbnvqxryxcdcnvbozc7u/Maniglia.png

•	Immagine Vetro= https://emerald-imaginative-spoonbill-973.mypinata.cloud/ipfs/bafybeifmehw7ebfkwm4jedaf34lhyswkfamxefkbnvqxryxcdcnvbozc7u/Vetro.png

Inizialmente il contratto è stato testato in ambiente Test Remix, verificando i vari parametri.
Dopo la compilazione il contratto è stato deployato e sono state testate le varie funzioni
Successivamente, è stato effettuato il deployment su rete testnet SEPOLIA. 
È stato possibile attraverso la richiesta di token test (sempre su tesnet), utilizzando come provider Metamask.

Attraverso lo scanner, è possibile vedere che il deployment è avvenuto in data 11/03/2025. 
Come da previsione,al momento del deployment  sono stati mintati nell’address del proprietario i relativi token. 
Il contratto funziona perfettamente.  

Questa è la Transaction Hash attraverso la quale sono stati ereditati i token test:
0x5f116103a11ee73a890fa03bcec8a4064570d6dd1fd5ef9cd84df39e1e2ba20e 

Smart Contract ERC1155
0xfc808e6A9FC2E67565d69D793f4046D7dcAe5B91

Sepolia Testnet Explorer
https://sepolia.etherscan.io/   


