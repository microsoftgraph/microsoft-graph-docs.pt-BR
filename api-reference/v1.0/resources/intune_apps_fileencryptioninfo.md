# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="e4700-101">Tipo de recurso fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="e4700-101">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="e4700-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e4700-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4700-103">Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.</span><span class="sxs-lookup"><span data-stu-id="e4700-103">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="e4700-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e4700-104">Properties</span></span>
|<span data-ttu-id="e4700-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e4700-105">Property</span></span>|<span data-ttu-id="e4700-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4700-106">Type</span></span>|<span data-ttu-id="e4700-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4700-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4700-108">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="e4700-108">encryptionKey</span></span>|<span data-ttu-id="e4700-109">Binária</span><span class="sxs-lookup"><span data-stu-id="e4700-109">Binary</span></span>|<span data-ttu-id="e4700-110">A chave usada para criptografar o conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="e4700-110">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="e4700-111">initializationVector</span><span class="sxs-lookup"><span data-stu-id="e4700-111">initializationVector</span></span>|<span data-ttu-id="e4700-112">Binária</span><span class="sxs-lookup"><span data-stu-id="e4700-112">Binary</span></span>|<span data-ttu-id="e4700-113">O vetor de inicialização usado para o algoritmo de criptografia.</span><span class="sxs-lookup"><span data-stu-id="e4700-113">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="e4700-114">mac</span><span class="sxs-lookup"><span data-stu-id="e4700-114">mac</span></span>|<span data-ttu-id="e4700-115">Binária</span><span class="sxs-lookup"><span data-stu-id="e4700-115">Binary</span></span>|<span data-ttu-id="e4700-116">O hash do conteúdo do arquivo criptografado + IV (hash conteúdo).</span><span class="sxs-lookup"><span data-stu-id="e4700-116">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="e4700-117">macKey</span><span class="sxs-lookup"><span data-stu-id="e4700-117">macKey</span></span>|<span data-ttu-id="e4700-118">Binária</span><span class="sxs-lookup"><span data-stu-id="e4700-118">Binary</span></span>|<span data-ttu-id="e4700-119">Chave usada para acessar mac.</span><span class="sxs-lookup"><span data-stu-id="e4700-119">The key used to get mac.</span></span>|
|<span data-ttu-id="e4700-120">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="e4700-120">profileIdentifier</span></span>|<span data-ttu-id="e4700-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4700-121">String</span></span>|<span data-ttu-id="e4700-122">O identificador de perfil.</span><span class="sxs-lookup"><span data-stu-id="e4700-122">The the profile identifier.</span></span>|
|<span data-ttu-id="e4700-123">fileDigest</span><span class="sxs-lookup"><span data-stu-id="e4700-123">fileDigest</span></span>|<span data-ttu-id="e4700-124">Binária</span><span class="sxs-lookup"><span data-stu-id="e4700-124">Binary</span></span>|<span data-ttu-id="e4700-125">O resumo de arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="e4700-125">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="e4700-126">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="e4700-126">fileDigestAlgorithm</span></span>|<span data-ttu-id="e4700-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4700-127">String</span></span>|<span data-ttu-id="e4700-128">O algoritmo de conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="e4700-128">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4700-129">Relações</span><span class="sxs-lookup"><span data-stu-id="e4700-129">Relationships</span></span>
<span data-ttu-id="e4700-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e4700-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e4700-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e4700-131">JSON Representation</span></span>
<span data-ttu-id="e4700-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e4700-132">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fileEncryptionInfo"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.fileEncryptionInfo",
  "encryptionKey": "binary",
  "initializationVector": "binary",
  "mac": "binary",
  "macKey": "binary",
  "profileIdentifier": "String",
  "fileDigest": "binary",
  "fileDigestAlgorithm": "String"
}
```



