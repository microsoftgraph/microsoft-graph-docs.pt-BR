# <a name="mobileapp-resource-type"></a><span data-ttu-id="c6aef-101">Tipo de recurso mobileApp</span><span class="sxs-lookup"><span data-stu-id="c6aef-101">mobileApp resource type</span></span>

> <span data-ttu-id="c6aef-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c6aef-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6aef-103">Uma classe abstrata que contém as propriedades base de aplicativos móveis do Intune.</span><span class="sxs-lookup"><span data-stu-id="c6aef-103">An abstract class containing the base properties for Intune mobile apps.</span></span>
## <a name="methods"></a><span data-ttu-id="c6aef-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="c6aef-104">Methods</span></span>
|<span data-ttu-id="c6aef-105">Método</span><span class="sxs-lookup"><span data-stu-id="c6aef-105">Method</span></span>|<span data-ttu-id="c6aef-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c6aef-106">Return Type</span></span>|<span data-ttu-id="c6aef-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6aef-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c6aef-108">Listar mobileApps</span><span class="sxs-lookup"><span data-stu-id="c6aef-108">List mobileApps</span></span>](../api/intune_apps_mobileapp_list.md)|<span data-ttu-id="c6aef-109">Coleção [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c6aef-109">[mobileApp](../resources/intune_apps_mobileapp.md) collection</span></span>|<span data-ttu-id="c6aef-110">Lista propriedades e relações dos objetos [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6aef-110">List properties and relationships of the [mobileApp](../resources/intune_apps_mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="c6aef-111">Obter mobileApp</span><span class="sxs-lookup"><span data-stu-id="c6aef-111">Get mobileApp</span></span>](../api/intune_apps_mobileapp_get.md)|[<span data-ttu-id="c6aef-112">mobileApp</span><span class="sxs-lookup"><span data-stu-id="c6aef-112">mobileApp</span></span>](../resources/intune_apps_mobileapp.md)|<span data-ttu-id="c6aef-113">Propriedades de leitura e relações do objeto [mobileApp](../resources/intune_apps_mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6aef-113">Read properties and relationships of the [mobileApp](../resources/intune_apps_mobileapp.md) object.</span></span>|
|[<span data-ttu-id="c6aef-114">ação assign</span><span class="sxs-lookup"><span data-stu-id="c6aef-114">assign action</span></span>](../api/intune_apps_mobileapp_assign.md)|<span data-ttu-id="c6aef-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c6aef-115">None</span></span>|<span data-ttu-id="c6aef-116">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c6aef-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c6aef-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c6aef-117">Properties</span></span>
|<span data-ttu-id="c6aef-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6aef-118">Property</span></span>|<span data-ttu-id="c6aef-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6aef-119">Type</span></span>|<span data-ttu-id="c6aef-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6aef-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6aef-121">id</span><span class="sxs-lookup"><span data-stu-id="c6aef-121">id</span></span>|<span data-ttu-id="c6aef-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6aef-122">String</span></span>|<span data-ttu-id="c6aef-123">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c6aef-123">Key of the entity.</span></span>|
|<span data-ttu-id="c6aef-124">displayName</span><span class="sxs-lookup"><span data-stu-id="c6aef-124">displayName</span></span>|<span data-ttu-id="c6aef-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6aef-125">String</span></span>|<span data-ttu-id="c6aef-126">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="c6aef-126">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="c6aef-127">description</span><span class="sxs-lookup"><span data-stu-id="c6aef-127">description</span></span>|<span data-ttu-id="c6aef-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6aef-128">String</span></span>|<span data-ttu-id="c6aef-129">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c6aef-129">The description of the app.</span></span>|
|<span data-ttu-id="c6aef-130">publisher</span><span class="sxs-lookup"><span data-stu-id="c6aef-130">publisher</span></span>|<span data-ttu-id="c6aef-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6aef-131">String</span></span>|<span data-ttu-id="c6aef-132">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c6aef-132">The publisher of the app.</span></span>|
|<span data-ttu-id="c6aef-133">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c6aef-133">largeIcon</span></span>|[<span data-ttu-id="c6aef-134">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c6aef-134">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="c6aef-135">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="c6aef-135">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="c6aef-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c6aef-136">createdDateTime</span></span>|<span data-ttu-id="c6aef-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6aef-137">DateTimeOffset</span></span>|<span data-ttu-id="c6aef-138">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c6aef-138">The date and time the app was created.</span></span>|
|<span data-ttu-id="c6aef-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c6aef-139">lastModifiedDateTime</span></span>|<span data-ttu-id="c6aef-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6aef-140">DateTimeOffset</span></span>|<span data-ttu-id="c6aef-141">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="c6aef-141">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="c6aef-142">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c6aef-142">isFeatured</span></span>|<span data-ttu-id="c6aef-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="c6aef-143">Boolean</span></span>|<span data-ttu-id="c6aef-144">O valor que indica se o aplicativo está marcado como em destaque pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="c6aef-144">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="c6aef-145">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c6aef-145">privacyInformationUrl</span></span>|<span data-ttu-id="c6aef-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6aef-146">String</span></span>|<span data-ttu-id="c6aef-147">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="c6aef-147">The privacy statement Url.</span></span>|
|<span data-ttu-id="c6aef-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c6aef-148">informationUrl</span></span>|<span data-ttu-id="c6aef-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6aef-149">String</span></span>|<span data-ttu-id="c6aef-150">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="c6aef-150">The more information Url.</span></span>|
|<span data-ttu-id="c6aef-151">owner</span><span class="sxs-lookup"><span data-stu-id="c6aef-151">owner</span></span>|<span data-ttu-id="c6aef-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6aef-152">String</span></span>|<span data-ttu-id="c6aef-153">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="c6aef-153">The owner of the app.</span></span>|
|<span data-ttu-id="c6aef-154">developer</span><span class="sxs-lookup"><span data-stu-id="c6aef-154">developer</span></span>|<span data-ttu-id="c6aef-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6aef-155">String</span></span>|<span data-ttu-id="c6aef-156">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c6aef-156">The developer of the app.</span></span>|
|<span data-ttu-id="c6aef-157">notes</span><span class="sxs-lookup"><span data-stu-id="c6aef-157">notes</span></span>|<span data-ttu-id="c6aef-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6aef-158">String</span></span>|<span data-ttu-id="c6aef-159">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c6aef-159">Notes for the app.</span></span>|
|<span data-ttu-id="c6aef-160">publishingState</span><span class="sxs-lookup"><span data-stu-id="c6aef-160">publishingState</span></span>|[<span data-ttu-id="c6aef-161">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c6aef-161">mobileAppPublishingState</span></span>](../resources/intune_apps_mobileapppublishingstate.md)|<span data-ttu-id="c6aef-p101">O estado de publicação do aplicativo. O aplicativo não pode ser atribuído a menos esteja publicado. Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="c6aef-p101">The publishing state for the app. The app cannot be assigned unless the app is published. The possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6aef-165">Relações</span><span class="sxs-lookup"><span data-stu-id="c6aef-165">Relationships</span></span>
|<span data-ttu-id="c6aef-166">Relação</span><span class="sxs-lookup"><span data-stu-id="c6aef-166">Relationship</span></span>|<span data-ttu-id="c6aef-167">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6aef-167">Type</span></span>|<span data-ttu-id="c6aef-168">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6aef-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6aef-169">categories</span><span class="sxs-lookup"><span data-stu-id="c6aef-169">categories</span></span>|<span data-ttu-id="c6aef-170">Coleção [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="c6aef-170">[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) collection</span></span>|<span data-ttu-id="c6aef-171">A lista de categorias para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c6aef-171">The list of categories for this app.</span></span>|
|<span data-ttu-id="c6aef-172">assignments</span><span class="sxs-lookup"><span data-stu-id="c6aef-172">assignments</span></span>|<span data-ttu-id="c6aef-173">Coleção [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c6aef-173">[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) collection</span></span>|<span data-ttu-id="c6aef-174">A lista de atribuições de grupo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="c6aef-174">The list of group assignments for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c6aef-175">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c6aef-175">JSON Representation</span></span>
<span data-ttu-id="c6aef-176">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c6aef-176">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "publishingState": "String"
}
```








