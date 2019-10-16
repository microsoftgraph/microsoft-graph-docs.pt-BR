---
title: Tipo de recurso mobileApp
description: Uma classe abstrata que contém as propriedades base de aplicativos móveis do Intune.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9688f0b4223fe0e1ec2e355c54f0efcbffdc2573
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538718"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="23be5-103">Tipo de recurso mobileApp</span><span class="sxs-lookup"><span data-stu-id="23be5-103">mobileApp resource type</span></span>

> <span data-ttu-id="23be5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="23be5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23be5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="23be5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23be5-106">Uma classe abstrata que contém as propriedades base de aplicativos móveis do Intune.</span><span class="sxs-lookup"><span data-stu-id="23be5-106">An abstract class containing the base properties for Intune mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="23be5-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="23be5-107">Methods</span></span>
|<span data-ttu-id="23be5-108">Método</span><span class="sxs-lookup"><span data-stu-id="23be5-108">Method</span></span>|<span data-ttu-id="23be5-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="23be5-109">Return Type</span></span>|<span data-ttu-id="23be5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="23be5-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="23be5-111">Listar mobileApps</span><span class="sxs-lookup"><span data-stu-id="23be5-111">List mobileApps</span></span>](../api/intune-shared-mobileapp-list.md)|<span data-ttu-id="23be5-112">Coleção [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="23be5-112">[mobileApp](../resources/intune-shared-mobileapp.md) collection</span></span>|<span data-ttu-id="23be5-113">Lista propriedades e relações dos objetos [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="23be5-113">List properties and relationships of the [mobileApp](../resources/intune-shared-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="23be5-114">Obter mobileApp</span><span class="sxs-lookup"><span data-stu-id="23be5-114">Get mobileApp</span></span>](../api/intune-shared-mobileapp-get.md)|[<span data-ttu-id="23be5-115">mobileApp</span><span class="sxs-lookup"><span data-stu-id="23be5-115">mobileApp</span></span>](../resources/intune-shared-mobileapp.md)|<span data-ttu-id="23be5-116">Propriedades de leitura e relações do objeto [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="23be5-116">Read properties and relationships of the [mobileApp](../resources/intune-shared-mobileapp.md) object.</span></span>|
|<span data-ttu-id="23be5-117">**Apps**</span><span class="sxs-lookup"><span data-stu-id="23be5-117">**Apps**</span></span>|
|[<span data-ttu-id="23be5-118">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="23be5-118">assign action</span></span>](../api/intune-shared-mobileapp-assign.md)|<span data-ttu-id="23be5-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="23be5-119">None</span></span>|<span data-ttu-id="23be5-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="23be5-120">Not yet documented</span></span>|
|[<span data-ttu-id="23be5-121">função getMobileAppCount</span><span class="sxs-lookup"><span data-stu-id="23be5-121">getMobileAppCount function</span></span>](../api/intune-shared-mobileapp-getmobileappcount.md)|<span data-ttu-id="23be5-122">Int64</span><span class="sxs-lookup"><span data-stu-id="23be5-122">Int64</span></span>|<span data-ttu-id="23be5-123">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="23be5-123">Not yet documented</span></span>|
|[<span data-ttu-id="23be5-124">função getTopMobileApps</span><span class="sxs-lookup"><span data-stu-id="23be5-124">getTopMobileApps function</span></span>](../api/intune-shared-mobileapp-gettopmobileapps.md)|<span data-ttu-id="23be5-125">Coleção [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="23be5-125">[mobileApp](../resources/intune-shared-mobileapp.md) collection</span></span>|<span data-ttu-id="23be5-126">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="23be5-126">Not yet documented</span></span>|
|[<span data-ttu-id="23be5-127">ação updateRelationships</span><span class="sxs-lookup"><span data-stu-id="23be5-127">updateRelationships action</span></span>](../api/intune-shared-mobileapp-updaterelationships.md)|<span data-ttu-id="23be5-128">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="23be5-128">None</span></span>|<span data-ttu-id="23be5-129">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="23be5-129">Not yet documented</span></span>|
|[<span data-ttu-id="23be5-130">função getRelatedAppStates</span><span class="sxs-lookup"><span data-stu-id="23be5-130">getRelatedAppStates function</span></span>](../api/intune-shared-mobileapp-getrelatedappstates.md)|<span data-ttu-id="23be5-131">coleção [mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md)</span><span class="sxs-lookup"><span data-stu-id="23be5-131">[mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) collection</span></span>|<span data-ttu-id="23be5-132">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="23be5-132">Not yet documented</span></span>|
|<span data-ttu-id="23be5-133">**Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="23be5-133">**Policy Set**</span></span>|
|[<span data-ttu-id="23be5-134">ação hasPayloadLinks</span><span class="sxs-lookup"><span data-stu-id="23be5-134">hasPayloadLinks action</span></span>](../api/intune-shared-mobileapp-haspayloadlinks.md)|<span data-ttu-id="23be5-135">coleção [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)</span><span class="sxs-lookup"><span data-stu-id="23be5-135">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="23be5-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="23be5-136">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="23be5-137">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23be5-137">Properties</span></span>
|<span data-ttu-id="23be5-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23be5-138">Property</span></span>|<span data-ttu-id="23be5-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="23be5-139">Type</span></span>|<span data-ttu-id="23be5-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="23be5-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23be5-141">id</span><span class="sxs-lookup"><span data-stu-id="23be5-141">id</span></span>|<span data-ttu-id="23be5-142">String</span><span class="sxs-lookup"><span data-stu-id="23be5-142">String</span></span>|<span data-ttu-id="23be5-143">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="23be5-143">Key of the entity.</span></span>|
|<span data-ttu-id="23be5-144">displayName</span><span class="sxs-lookup"><span data-stu-id="23be5-144">displayName</span></span>|<span data-ttu-id="23be5-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23be5-145">String</span></span>|<span data-ttu-id="23be5-146">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="23be5-146">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="23be5-147">description</span><span class="sxs-lookup"><span data-stu-id="23be5-147">description</span></span>|<span data-ttu-id="23be5-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23be5-148">String</span></span>|<span data-ttu-id="23be5-149">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="23be5-149">The description of the app.</span></span>|
|<span data-ttu-id="23be5-150">publisher</span><span class="sxs-lookup"><span data-stu-id="23be5-150">publisher</span></span>|<span data-ttu-id="23be5-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23be5-151">String</span></span>|<span data-ttu-id="23be5-152">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="23be5-152">The publisher of the app.</span></span>|
|<span data-ttu-id="23be5-153">largeIcon</span><span class="sxs-lookup"><span data-stu-id="23be5-153">largeIcon</span></span>|[<span data-ttu-id="23be5-154">mimeContent</span><span class="sxs-lookup"><span data-stu-id="23be5-154">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="23be5-155">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="23be5-155">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="23be5-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="23be5-156">createdDateTime</span></span>|<span data-ttu-id="23be5-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23be5-157">DateTimeOffset</span></span>|<span data-ttu-id="23be5-158">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="23be5-158">The date and time the app was created.</span></span>|
|<span data-ttu-id="23be5-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23be5-159">lastModifiedDateTime</span></span>|<span data-ttu-id="23be5-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23be5-160">DateTimeOffset</span></span>|<span data-ttu-id="23be5-161">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="23be5-161">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="23be5-162">isFeatured</span><span class="sxs-lookup"><span data-stu-id="23be5-162">isFeatured</span></span>|<span data-ttu-id="23be5-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="23be5-163">Boolean</span></span>|<span data-ttu-id="23be5-164">O valor que indica se o aplicativo está marcado como em destaque pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="23be5-164">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="23be5-165">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="23be5-165">privacyInformationUrl</span></span>|<span data-ttu-id="23be5-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23be5-166">String</span></span>|<span data-ttu-id="23be5-167">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="23be5-167">The privacy statement Url.</span></span>|
|<span data-ttu-id="23be5-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="23be5-168">informationUrl</span></span>|<span data-ttu-id="23be5-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23be5-169">String</span></span>|<span data-ttu-id="23be5-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="23be5-170">The more information Url.</span></span>|
|<span data-ttu-id="23be5-171">owner</span><span class="sxs-lookup"><span data-stu-id="23be5-171">owner</span></span>|<span data-ttu-id="23be5-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23be5-172">String</span></span>|<span data-ttu-id="23be5-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="23be5-173">The owner of the app.</span></span>|
|<span data-ttu-id="23be5-174">developer</span><span class="sxs-lookup"><span data-stu-id="23be5-174">developer</span></span>|<span data-ttu-id="23be5-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23be5-175">String</span></span>|<span data-ttu-id="23be5-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="23be5-176">The developer of the app.</span></span>|
|<span data-ttu-id="23be5-177">notes</span><span class="sxs-lookup"><span data-stu-id="23be5-177">notes</span></span>|<span data-ttu-id="23be5-178">String</span><span class="sxs-lookup"><span data-stu-id="23be5-178">String</span></span>|<span data-ttu-id="23be5-179">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="23be5-179">Notes for the app.</span></span>|
|<span data-ttu-id="23be5-180">uploadState</span><span class="sxs-lookup"><span data-stu-id="23be5-180">uploadState</span></span>|<span data-ttu-id="23be5-181">Int32</span><span class="sxs-lookup"><span data-stu-id="23be5-181">Int32</span></span>|<span data-ttu-id="23be5-182">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="23be5-182">The upload state.</span></span>|
|<span data-ttu-id="23be5-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="23be5-183">publishingState</span></span>|[<span data-ttu-id="23be5-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="23be5-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="23be5-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="23be5-185">The publishing state for the app.</span></span> <span data-ttu-id="23be5-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="23be5-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="23be5-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="23be5-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="23be5-188">isAssigned</span><span class="sxs-lookup"><span data-stu-id="23be5-188">isAssigned</span></span>|<span data-ttu-id="23be5-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="23be5-189">Boolean</span></span>|<span data-ttu-id="23be5-190">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="23be5-190">The value indicating whether the app is assigned to at least one group.</span></span>|
|<span data-ttu-id="23be5-191">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="23be5-191">roleScopeTagIds</span></span>|<span data-ttu-id="23be5-192">String collection</span><span class="sxs-lookup"><span data-stu-id="23be5-192">String collection</span></span>|<span data-ttu-id="23be5-193">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="23be5-193">List of scope tag ids for this mobile app.</span></span>|
|<span data-ttu-id="23be5-194">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="23be5-194">dependentAppCount</span></span>|<span data-ttu-id="23be5-195">Int32</span><span class="sxs-lookup"><span data-stu-id="23be5-195">Int32</span></span>|<span data-ttu-id="23be5-196">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="23be5-196">The total number of dependencies the child app has.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23be5-197">Relações</span><span class="sxs-lookup"><span data-stu-id="23be5-197">Relationships</span></span>
|<span data-ttu-id="23be5-198">Relação</span><span class="sxs-lookup"><span data-stu-id="23be5-198">Relationship</span></span>|<span data-ttu-id="23be5-199">Tipo</span><span class="sxs-lookup"><span data-stu-id="23be5-199">Type</span></span>|<span data-ttu-id="23be5-200">Descrição</span><span class="sxs-lookup"><span data-stu-id="23be5-200">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23be5-201">**Apps**</span><span class="sxs-lookup"><span data-stu-id="23be5-201">**Apps**</span></span>|
|<span data-ttu-id="23be5-202">categories</span><span class="sxs-lookup"><span data-stu-id="23be5-202">categories</span></span>|<span data-ttu-id="23be5-203">Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="23be5-203">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="23be5-204">A lista de categorias para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="23be5-204">The list of categories for this app.</span></span>|
|<span data-ttu-id="23be5-205">assignments</span><span class="sxs-lookup"><span data-stu-id="23be5-205">assignments</span></span>|<span data-ttu-id="23be5-206">Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="23be5-206">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="23be5-207">A lista de atribuições de grupo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="23be5-207">The list of group assignments for this mobile app.</span></span>|
|<span data-ttu-id="23be5-208">installSummary</span><span class="sxs-lookup"><span data-stu-id="23be5-208">installSummary</span></span>|[<span data-ttu-id="23be5-209">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="23be5-209">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="23be5-210">Resumo de instalação do aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="23be5-210">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="23be5-211">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="23be5-211">deviceStatuses</span></span>|<span data-ttu-id="23be5-212">coleção [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="23be5-212">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="23be5-213">A lista de Estados de instalação para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="23be5-213">The list of installation states for this mobile app.</span></span>|
|<span data-ttu-id="23be5-214">userStatuses</span><span class="sxs-lookup"><span data-stu-id="23be5-214">userStatuses</span></span>|<span data-ttu-id="23be5-215">coleção [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="23be5-215">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="23be5-216">A lista de Estados de instalação para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="23be5-216">The list of installation states for this mobile app.</span></span>|
|<span data-ttu-id="23be5-217">relações</span><span class="sxs-lookup"><span data-stu-id="23be5-217">relationships</span></span>|<span data-ttu-id="23be5-218">coleção [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="23be5-218">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="23be5-219">Lista de relações para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="23be5-219">List of relationships for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="23be5-220">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23be5-220">JSON Representation</span></span>
<span data-ttu-id="23be5-221">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23be5-221">Here is a JSON representation of the resource.</span></span>
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



