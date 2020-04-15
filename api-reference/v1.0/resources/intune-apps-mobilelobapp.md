---
title: Tipo de recurso mobileLobApp
description: Uma classe base abstrata que contém propriedades para a toda a linha móvel de aplicativos de negócios.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1003d8e7e2ef0295f7635b478a0e5de32cf3414a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439649"
---
# <a name="mobilelobapp-resource-type"></a><span data-ttu-id="730d8-103">Tipo de recurso mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="730d8-103">mobileLobApp resource type</span></span>

<span data-ttu-id="730d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="730d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="730d8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="730d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="730d8-106">Uma classe base abstrata que contém propriedades para a toda a linha móvel de aplicativos de negócios.</span><span class="sxs-lookup"><span data-stu-id="730d8-106">An abstract base class containing properties for all mobile line of business apps.</span></span>


<span data-ttu-id="730d8-107">Herda de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="730d8-107">Inherits from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="730d8-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="730d8-108">Methods</span></span>
|<span data-ttu-id="730d8-109">Método</span><span class="sxs-lookup"><span data-stu-id="730d8-109">Method</span></span>|<span data-ttu-id="730d8-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="730d8-110">Return Type</span></span>|<span data-ttu-id="730d8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="730d8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="730d8-112">Listar mobileLobApps</span><span class="sxs-lookup"><span data-stu-id="730d8-112">List mobileLobApps</span></span>](../api/intune-apps-mobilelobapp-list.md)|<span data-ttu-id="730d8-113">Coleção [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="730d8-113">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) collection</span></span>|<span data-ttu-id="730d8-114">Lista propriedades e relações dos objetos [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="730d8-114">List properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) objects.</span></span>|
|[<span data-ttu-id="730d8-115">Obter mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="730d8-115">Get mobileLobApp</span></span>](../api/intune-apps-mobilelobapp-get.md)|[<span data-ttu-id="730d8-116">mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="730d8-116">mobileLobApp</span></span>](../resources/intune-apps-mobilelobapp.md)|<span data-ttu-id="730d8-117">Propriedades de leitura e relações do objeto [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="730d8-117">Read properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="730d8-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="730d8-118">Properties</span></span>
|<span data-ttu-id="730d8-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="730d8-119">Property</span></span>|<span data-ttu-id="730d8-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="730d8-120">Type</span></span>|<span data-ttu-id="730d8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="730d8-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="730d8-122">id</span><span class="sxs-lookup"><span data-stu-id="730d8-122">id</span></span>|<span data-ttu-id="730d8-123">String</span><span class="sxs-lookup"><span data-stu-id="730d8-123">String</span></span>|<span data-ttu-id="730d8-124">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="730d8-124">Key of the entity.</span></span> <span data-ttu-id="730d8-125">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="730d8-125">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="730d8-126">displayName</span><span class="sxs-lookup"><span data-stu-id="730d8-126">displayName</span></span>|<span data-ttu-id="730d8-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="730d8-127">String</span></span>|<span data-ttu-id="730d8-128">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="730d8-128">The admin provided or imported title of the app.</span></span> <span data-ttu-id="730d8-129">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="730d8-129">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="730d8-130">description</span><span class="sxs-lookup"><span data-stu-id="730d8-130">description</span></span>|<span data-ttu-id="730d8-131">String</span><span class="sxs-lookup"><span data-stu-id="730d8-131">String</span></span>|<span data-ttu-id="730d8-132">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="730d8-132">The description of the app.</span></span> <span data-ttu-id="730d8-133">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="730d8-133">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="730d8-134">publicador</span><span class="sxs-lookup"><span data-stu-id="730d8-134">publisher</span></span>|<span data-ttu-id="730d8-135">String</span><span class="sxs-lookup"><span data-stu-id="730d8-135">String</span></span>|<span data-ttu-id="730d8-136">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="730d8-136">The publisher of the app.</span></span> <span data-ttu-id="730d8-137">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="730d8-137">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="730d8-138">largeIcon</span><span class="sxs-lookup"><span data-stu-id="730d8-138">largeIcon</span></span>|[<span data-ttu-id="730d8-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="730d8-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="730d8-140">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="730d8-140">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="730d8-141">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="730d8-141">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="730d8-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="730d8-142">createdDateTime</span></span>|<span data-ttu-id="730d8-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="730d8-143">DateTimeOffset</span></span>|<span data-ttu-id="730d8-144">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="730d8-144">The date and time the app was created.</span></span> <span data-ttu-id="730d8-145">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="730d8-145">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="730d8-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="730d8-146">lastModifiedDateTime</span></span>|<span data-ttu-id="730d8-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="730d8-147">DateTimeOffset</span></span>|<span data-ttu-id="730d8-148">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="730d8-148">The date and time the app was last modified.</span></span> <span data-ttu-id="730d8-149">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="730d8-149">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="730d8-150">isFeatured</span><span class="sxs-lookup"><span data-stu-id="730d8-150">isFeatured</span></span>|<span data-ttu-id="730d8-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="730d8-151">Boolean</span></span>|<span data-ttu-id="730d8-152">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="730d8-152">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="730d8-153">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="730d8-153">privacyInformationUrl</span></span>|<span data-ttu-id="730d8-154">String</span><span class="sxs-lookup"><span data-stu-id="730d8-154">String</span></span>|<span data-ttu-id="730d8-155">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="730d8-155">The privacy statement Url.</span></span> <span data-ttu-id="730d8-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="730d8-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="730d8-157">informationUrl</span><span class="sxs-lookup"><span data-stu-id="730d8-157">informationUrl</span></span>|<span data-ttu-id="730d8-158">String</span><span class="sxs-lookup"><span data-stu-id="730d8-158">String</span></span>|<span data-ttu-id="730d8-159">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="730d8-159">The more information Url.</span></span> <span data-ttu-id="730d8-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="730d8-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="730d8-161">owner</span><span class="sxs-lookup"><span data-stu-id="730d8-161">owner</span></span>|<span data-ttu-id="730d8-162">String</span><span class="sxs-lookup"><span data-stu-id="730d8-162">String</span></span>|<span data-ttu-id="730d8-163">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="730d8-163">The owner of the app.</span></span> <span data-ttu-id="730d8-164">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="730d8-164">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="730d8-165">developer</span><span class="sxs-lookup"><span data-stu-id="730d8-165">developer</span></span>|<span data-ttu-id="730d8-166">String</span><span class="sxs-lookup"><span data-stu-id="730d8-166">String</span></span>|<span data-ttu-id="730d8-167">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="730d8-167">The developer of the app.</span></span> <span data-ttu-id="730d8-168">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="730d8-168">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="730d8-169">notes</span><span class="sxs-lookup"><span data-stu-id="730d8-169">notes</span></span>|<span data-ttu-id="730d8-170">String</span><span class="sxs-lookup"><span data-stu-id="730d8-170">String</span></span>|<span data-ttu-id="730d8-171">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="730d8-171">Notes for the app.</span></span> <span data-ttu-id="730d8-172">Herdada de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="730d8-172">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="730d8-173">publishingState</span><span class="sxs-lookup"><span data-stu-id="730d8-173">publishingState</span></span>|[<span data-ttu-id="730d8-174">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="730d8-174">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="730d8-175">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="730d8-175">The publishing state for the app.</span></span> <span data-ttu-id="730d8-176">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="730d8-176">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="730d8-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="730d8-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="730d8-178">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="730d8-178">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="730d8-179">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="730d8-179">committedContentVersion</span></span>|<span data-ttu-id="730d8-180">String</span><span class="sxs-lookup"><span data-stu-id="730d8-180">String</span></span>|<span data-ttu-id="730d8-181">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="730d8-181">The internal committed content version.</span></span>|
|<span data-ttu-id="730d8-182">fileName</span><span class="sxs-lookup"><span data-stu-id="730d8-182">fileName</span></span>|<span data-ttu-id="730d8-183">String</span><span class="sxs-lookup"><span data-stu-id="730d8-183">String</span></span>|<span data-ttu-id="730d8-184">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="730d8-184">The name of the main Lob application file.</span></span>|
|<span data-ttu-id="730d8-185">size</span><span class="sxs-lookup"><span data-stu-id="730d8-185">size</span></span>|<span data-ttu-id="730d8-186">Int64</span><span class="sxs-lookup"><span data-stu-id="730d8-186">Int64</span></span>|<span data-ttu-id="730d8-187">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="730d8-187">The total size, including all uploaded files.</span></span>|

## <a name="relationships"></a><span data-ttu-id="730d8-188">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="730d8-188">Relationships</span></span>
|<span data-ttu-id="730d8-189">Relação</span><span class="sxs-lookup"><span data-stu-id="730d8-189">Relationship</span></span>|<span data-ttu-id="730d8-190">Tipo</span><span class="sxs-lookup"><span data-stu-id="730d8-190">Type</span></span>|<span data-ttu-id="730d8-191">Descrição</span><span class="sxs-lookup"><span data-stu-id="730d8-191">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="730d8-192">categories</span><span class="sxs-lookup"><span data-stu-id="730d8-192">categories</span></span>|<span data-ttu-id="730d8-193">Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="730d8-193">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="730d8-194">A lista de categorias para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="730d8-194">The list of categories for this app.</span></span> <span data-ttu-id="730d8-195">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="730d8-195">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="730d8-196">assignments</span><span class="sxs-lookup"><span data-stu-id="730d8-196">assignments</span></span>|<span data-ttu-id="730d8-197">Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="730d8-197">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="730d8-198">A lista de atribuições de grupo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="730d8-198">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="730d8-199">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="730d8-199">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="730d8-200">contentVersions</span><span class="sxs-lookup"><span data-stu-id="730d8-200">contentVersions</span></span>|<span data-ttu-id="730d8-201">Coleção [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="730d8-201">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="730d8-202">A lista das versões de conteúdo deste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="730d8-202">The list of content versions for this app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="730d8-203">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="730d8-203">JSON Representation</span></span>
<span data-ttu-id="730d8-204">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="730d8-204">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileLobApp",
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
  "publishingState": "String",
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024
}
```







