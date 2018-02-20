# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="e1a2a-101">Tipo de recurso bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="e1a2a-101">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="e1a2a-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e1a2a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1a2a-103">Políticas da unidade removível do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="e1a2a-103">BitLocker Removable Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="e1a2a-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1a2a-104">Properties</span></span>
|<span data-ttu-id="e1a2a-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1a2a-105">Property</span></span>|<span data-ttu-id="e1a2a-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1a2a-106">Type</span></span>|<span data-ttu-id="e1a2a-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1a2a-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1a2a-108">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="e1a2a-108">encryptionMethod</span></span>|<span data-ttu-id="e1a2a-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1a2a-109">String</span></span>|<span data-ttu-id="e1a2a-110">Selecione o método de criptografia para unidades removíveis.</span><span class="sxs-lookup"><span data-stu-id="e1a2a-110">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="e1a2a-111">Os valores possíveis são: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="e1a2a-111">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="e1a2a-112">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="e1a2a-112">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="e1a2a-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="e1a2a-113">Boolean</span></span>|<span data-ttu-id="e1a2a-114">Indica se o acesso de gravação deve ser bloqueado para dispositivos configurados em outra organização.</span><span class="sxs-lookup"><span data-stu-id="e1a2a-114">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="e1a2a-115">Se requireEncryptionForWriteAccess for false, esse valor não será afetado.</span><span class="sxs-lookup"><span data-stu-id="e1a2a-115">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="e1a2a-116">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="e1a2a-116">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="e1a2a-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="e1a2a-117">Boolean</span></span>|<span data-ttu-id="e1a2a-118">Essa configuração de política determina se a proteção BitLocker é necessária para que unidades de dados removíveis sejam graváveis em um computador.</span><span class="sxs-lookup"><span data-stu-id="e1a2a-118">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1a2a-119">Relações</span><span class="sxs-lookup"><span data-stu-id="e1a2a-119">Relationships</span></span>
<span data-ttu-id="e1a2a-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e1a2a-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e1a2a-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1a2a-121">JSON Representation</span></span>
<span data-ttu-id="e1a2a-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1a2a-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRemovableDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "blockCrossOrganizationWriteAccess": true
}
```



