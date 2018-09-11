# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="5d8c1-101">Tipo de recurso bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="5d8c1-101">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="5d8c1-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5d8c1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d8c1-103">Políticas da unidade removível do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="5d8c1-103">BitLocker Removable Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="5d8c1-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5d8c1-104">Properties</span></span>
|<span data-ttu-id="5d8c1-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5d8c1-105">Property</span></span>|<span data-ttu-id="5d8c1-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d8c1-106">Type</span></span>|<span data-ttu-id="5d8c1-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d8c1-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d8c1-108">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="5d8c1-108">encryptionMethod</span></span>|[<span data-ttu-id="5d8c1-109">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="5d8c1-109">bitLockerEncryptionMethod</span></span>](../resources/intune_deviceconfig_bitlockerencryptionmethod.md)|<span data-ttu-id="5d8c1-p101">Seleciona o método de criptografia para unidades removíveis. Os valores possíveis são: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="5d8c1-p101">Select the encryption method for removable  drives. The possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="5d8c1-112">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="5d8c1-112">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="5d8c1-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="5d8c1-113">Boolean</span></span>|<span data-ttu-id="5d8c1-114">Indica se o acesso de gravação deve ser bloqueado para dispositivos configurados em outra organização.</span><span class="sxs-lookup"><span data-stu-id="5d8c1-114">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="5d8c1-115">Se requireEncryptionForWriteAccess for false, esse valor não será afetado.</span><span class="sxs-lookup"><span data-stu-id="5d8c1-115">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="5d8c1-116">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="5d8c1-116">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="5d8c1-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="5d8c1-117">Boolean</span></span>|<span data-ttu-id="5d8c1-118">Essa configuração de política determina se a proteção BitLocker é necessária para que unidades de dados removíveis sejam graváveis em um computador.</span><span class="sxs-lookup"><span data-stu-id="5d8c1-118">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d8c1-119">Relações</span><span class="sxs-lookup"><span data-stu-id="5d8c1-119">Relationships</span></span>
<span data-ttu-id="5d8c1-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5d8c1-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5d8c1-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5d8c1-121">JSON Representation</span></span>
<span data-ttu-id="5d8c1-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5d8c1-122">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRemovableDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "blockCrossOrganizationWriteAccess": true
}
```








