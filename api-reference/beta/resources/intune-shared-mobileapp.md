---
title: Tipo de recurso mobileApp
description: Uma classe abstrata que contém as propriedades base de aplicativos móveis do Intune.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ca889aadfe5ce3a2bdbb7c2409db0b2ddec451af
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523622"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="48418-103">Tipo de recurso mobileApp</span><span class="sxs-lookup"><span data-stu-id="48418-103">mobileApp resource type</span></span>

<span data-ttu-id="48418-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="48418-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="48418-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="48418-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48418-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="48418-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48418-107">Uma classe abstrata que contém as propriedades base de aplicativos móveis do Intune.</span><span class="sxs-lookup"><span data-stu-id="48418-107">An abstract class containing the base properties for Intune mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="48418-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="48418-108">Methods</span></span>
|<span data-ttu-id="48418-109">Método</span><span class="sxs-lookup"><span data-stu-id="48418-109">Method</span></span>|<span data-ttu-id="48418-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="48418-110">Return Type</span></span>|<span data-ttu-id="48418-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="48418-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="48418-112">Listar mobileApps</span><span class="sxs-lookup"><span data-stu-id="48418-112">List mobileApps</span></span>](../api/intune-shared-mobileapp-list.md)|<span data-ttu-id="48418-113">Coleção [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48418-113">[mobileApp](../resources/intune-shared-mobileapp.md) collection</span></span>|<span data-ttu-id="48418-114">Lista propriedades e relações dos objetos [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48418-114">List properties and relationships of the [mobileApp](../resources/intune-shared-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="48418-115">Obter mobileApp</span><span class="sxs-lookup"><span data-stu-id="48418-115">Get mobileApp</span></span>](../api/intune-shared-mobileapp-get.md)|[<span data-ttu-id="48418-116">mobileApp</span><span class="sxs-lookup"><span data-stu-id="48418-116">mobileApp</span></span>](../resources/intune-shared-mobileapp.md)|<span data-ttu-id="48418-117">Propriedades de leitura e relações do objeto [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="48418-117">Read properties and relationships of the [mobileApp](../resources/intune-shared-mobileapp.md) object.</span></span>|
|<span data-ttu-id="48418-118">**Apps**</span><span class="sxs-lookup"><span data-stu-id="48418-118">**Apps**</span></span>|
|[<span data-ttu-id="48418-119">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="48418-119">assign action</span></span>](../api/intune-shared-mobileapp-assign.md)|<span data-ttu-id="48418-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="48418-120">None</span></span>|<span data-ttu-id="48418-121">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="48418-121">Not yet documented</span></span>|
|[<span data-ttu-id="48418-122">função getMobileAppCount</span><span class="sxs-lookup"><span data-stu-id="48418-122">getMobileAppCount function</span></span>](../api/intune-shared-mobileapp-getmobileappcount.md)|<span data-ttu-id="48418-123">Int64</span><span class="sxs-lookup"><span data-stu-id="48418-123">Int64</span></span>|<span data-ttu-id="48418-124">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="48418-124">Not yet documented</span></span>|
|[<span data-ttu-id="48418-125">função getTopMobileApps</span><span class="sxs-lookup"><span data-stu-id="48418-125">getTopMobileApps function</span></span>](../api/intune-shared-mobileapp-gettopmobileapps.md)|<span data-ttu-id="48418-126">Coleção [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48418-126">[mobileApp](../resources/intune-shared-mobileapp.md) collection</span></span>|<span data-ttu-id="48418-127">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="48418-127">Not yet documented</span></span>|
|[<span data-ttu-id="48418-128">ação updateRelationships</span><span class="sxs-lookup"><span data-stu-id="48418-128">updateRelationships action</span></span>](../api/intune-shared-mobileapp-updaterelationships.md)|<span data-ttu-id="48418-129">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="48418-129">None</span></span>|<span data-ttu-id="48418-130">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="48418-130">Not yet documented</span></span>|
|[<span data-ttu-id="48418-131">função getRelatedAppStates</span><span class="sxs-lookup"><span data-stu-id="48418-131">getRelatedAppStates function</span></span>](../api/intune-shared-mobileapp-getrelatedappstates.md)|<span data-ttu-id="48418-132">coleção [mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md)</span><span class="sxs-lookup"><span data-stu-id="48418-132">[mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) collection</span></span>|<span data-ttu-id="48418-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="48418-133">Not yet documented</span></span>|
|<span data-ttu-id="48418-134">**Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="48418-134">**Policy Set**</span></span>|
|[<span data-ttu-id="48418-135">ação hasPayloadLinks</span><span class="sxs-lookup"><span data-stu-id="48418-135">hasPayloadLinks action</span></span>](../api/intune-shared-mobileapp-haspayloadlinks.md)|<span data-ttu-id="48418-136">coleção [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)</span><span class="sxs-lookup"><span data-stu-id="48418-136">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="48418-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="48418-137">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="48418-138">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48418-138">Properties</span></span>
|<span data-ttu-id="48418-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48418-139">Property</span></span>|<span data-ttu-id="48418-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="48418-140">Type</span></span>|<span data-ttu-id="48418-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="48418-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48418-142">id</span><span class="sxs-lookup"><span data-stu-id="48418-142">id</span></span>|<span data-ttu-id="48418-143">String</span><span class="sxs-lookup"><span data-stu-id="48418-143">String</span></span>|<span data-ttu-id="48418-144">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="48418-144">Key of the entity.</span></span>|
|<span data-ttu-id="48418-145">displayName</span><span class="sxs-lookup"><span data-stu-id="48418-145">displayName</span></span>|<span data-ttu-id="48418-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="48418-146">String</span></span>|<span data-ttu-id="48418-147">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="48418-147">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="48418-148">description</span><span class="sxs-lookup"><span data-stu-id="48418-148">description</span></span>|<span data-ttu-id="48418-149">String</span><span class="sxs-lookup"><span data-stu-id="48418-149">String</span></span>|<span data-ttu-id="48418-150">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="48418-150">The description of the app.</span></span>|
|<span data-ttu-id="48418-151">publisher</span><span class="sxs-lookup"><span data-stu-id="48418-151">publisher</span></span>|<span data-ttu-id="48418-152">String</span><span class="sxs-lookup"><span data-stu-id="48418-152">String</span></span>|<span data-ttu-id="48418-153">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="48418-153">The publisher of the app.</span></span>|
|<span data-ttu-id="48418-154">largeIcon</span><span class="sxs-lookup"><span data-stu-id="48418-154">largeIcon</span></span>|[<span data-ttu-id="48418-155">mimeContent</span><span class="sxs-lookup"><span data-stu-id="48418-155">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="48418-156">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="48418-156">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="48418-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="48418-157">createdDateTime</span></span>|<span data-ttu-id="48418-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48418-158">DateTimeOffset</span></span>|<span data-ttu-id="48418-159">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="48418-159">The date and time the app was created.</span></span>|
|<span data-ttu-id="48418-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="48418-160">lastModifiedDateTime</span></span>|<span data-ttu-id="48418-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48418-161">DateTimeOffset</span></span>|<span data-ttu-id="48418-162">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="48418-162">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="48418-163">isFeatured</span><span class="sxs-lookup"><span data-stu-id="48418-163">isFeatured</span></span>|<span data-ttu-id="48418-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="48418-164">Boolean</span></span>|<span data-ttu-id="48418-165">O valor que indica se o aplicativo está marcado como em destaque pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="48418-165">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="48418-166">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="48418-166">privacyInformationUrl</span></span>|<span data-ttu-id="48418-167">String</span><span class="sxs-lookup"><span data-stu-id="48418-167">String</span></span>|<span data-ttu-id="48418-168">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="48418-168">The privacy statement Url.</span></span>|
|<span data-ttu-id="48418-169">informationUrl</span><span class="sxs-lookup"><span data-stu-id="48418-169">informationUrl</span></span>|<span data-ttu-id="48418-170">String</span><span class="sxs-lookup"><span data-stu-id="48418-170">String</span></span>|<span data-ttu-id="48418-171">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="48418-171">The more information Url.</span></span>|
|<span data-ttu-id="48418-172">owner</span><span class="sxs-lookup"><span data-stu-id="48418-172">owner</span></span>|<span data-ttu-id="48418-173">String</span><span class="sxs-lookup"><span data-stu-id="48418-173">String</span></span>|<span data-ttu-id="48418-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="48418-174">The owner of the app.</span></span>|
|<span data-ttu-id="48418-175">developer</span><span class="sxs-lookup"><span data-stu-id="48418-175">developer</span></span>|<span data-ttu-id="48418-176">String</span><span class="sxs-lookup"><span data-stu-id="48418-176">String</span></span>|<span data-ttu-id="48418-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="48418-177">The developer of the app.</span></span>|
|<span data-ttu-id="48418-178">notes</span><span class="sxs-lookup"><span data-stu-id="48418-178">notes</span></span>|<span data-ttu-id="48418-179">String</span><span class="sxs-lookup"><span data-stu-id="48418-179">String</span></span>|<span data-ttu-id="48418-180">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="48418-180">Notes for the app.</span></span>|
|<span data-ttu-id="48418-181">uploadState</span><span class="sxs-lookup"><span data-stu-id="48418-181">uploadState</span></span>|<span data-ttu-id="48418-182">Int32</span><span class="sxs-lookup"><span data-stu-id="48418-182">Int32</span></span>|<span data-ttu-id="48418-183">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="48418-183">The upload state.</span></span>|
|<span data-ttu-id="48418-184">publishingState</span><span class="sxs-lookup"><span data-stu-id="48418-184">publishingState</span></span>|[<span data-ttu-id="48418-185">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="48418-185">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="48418-186">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="48418-186">The publishing state for the app.</span></span> <span data-ttu-id="48418-187">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="48418-187">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="48418-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="48418-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="48418-189">isAssigned</span><span class="sxs-lookup"><span data-stu-id="48418-189">isAssigned</span></span>|<span data-ttu-id="48418-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="48418-190">Boolean</span></span>|<span data-ttu-id="48418-191">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="48418-191">The value indicating whether the app is assigned to at least one group.</span></span>|
|<span data-ttu-id="48418-192">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="48418-192">roleScopeTagIds</span></span>|<span data-ttu-id="48418-193">String collection</span><span class="sxs-lookup"><span data-stu-id="48418-193">String collection</span></span>|<span data-ttu-id="48418-194">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="48418-194">List of scope tag ids for this mobile app.</span></span>|
|<span data-ttu-id="48418-195">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="48418-195">dependentAppCount</span></span>|<span data-ttu-id="48418-196">Int32</span><span class="sxs-lookup"><span data-stu-id="48418-196">Int32</span></span>|<span data-ttu-id="48418-197">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="48418-197">The total number of dependencies the child app has.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48418-198">Relações</span><span class="sxs-lookup"><span data-stu-id="48418-198">Relationships</span></span>
|<span data-ttu-id="48418-199">Relação</span><span class="sxs-lookup"><span data-stu-id="48418-199">Relationship</span></span>|<span data-ttu-id="48418-200">Tipo</span><span class="sxs-lookup"><span data-stu-id="48418-200">Type</span></span>|<span data-ttu-id="48418-201">Descrição</span><span class="sxs-lookup"><span data-stu-id="48418-201">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48418-202">**Apps**</span><span class="sxs-lookup"><span data-stu-id="48418-202">**Apps**</span></span>|
|<span data-ttu-id="48418-203">categories</span><span class="sxs-lookup"><span data-stu-id="48418-203">categories</span></span>|<span data-ttu-id="48418-204">Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="48418-204">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="48418-205">A lista de categorias para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="48418-205">The list of categories for this app.</span></span>|
|<span data-ttu-id="48418-206">assignments</span><span class="sxs-lookup"><span data-stu-id="48418-206">assignments</span></span>|<span data-ttu-id="48418-207">Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="48418-207">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="48418-208">A lista de atribuições de grupo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="48418-208">The list of group assignments for this mobile app.</span></span>|
|<span data-ttu-id="48418-209">installSummary</span><span class="sxs-lookup"><span data-stu-id="48418-209">installSummary</span></span>|[<span data-ttu-id="48418-210">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="48418-210">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="48418-211">Resumo de instalação do aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="48418-211">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="48418-212">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="48418-212">deviceStatuses</span></span>|<span data-ttu-id="48418-213">coleção [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="48418-213">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="48418-214">A lista de Estados de instalação para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="48418-214">The list of installation states for this mobile app.</span></span>|
|<span data-ttu-id="48418-215">userStatuses</span><span class="sxs-lookup"><span data-stu-id="48418-215">userStatuses</span></span>|<span data-ttu-id="48418-216">coleção [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="48418-216">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="48418-217">A lista de Estados de instalação para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="48418-217">The list of installation states for this mobile app.</span></span>|
|<span data-ttu-id="48418-218">relações</span><span class="sxs-lookup"><span data-stu-id="48418-218">relationships</span></span>|<span data-ttu-id="48418-219">coleção [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="48418-219">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="48418-220">Lista de relações para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="48418-220">List of relationships for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="48418-221">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48418-221">JSON Representation</span></span>
<span data-ttu-id="48418-222">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="48418-222">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileApp"
}
-->
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
  "uploadState": 1024,
  "publishingState": "String",
  "isAssigned": true,
  "roleScopeTagIds": [
    "String"
  ],
  "dependentAppCount": 1024
}
```



