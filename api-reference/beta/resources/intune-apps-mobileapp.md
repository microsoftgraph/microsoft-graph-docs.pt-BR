---
title: Tipo de recurso mobileApp
description: Uma classe abstrata que contém as propriedades base de aplicativos móveis do Intune.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 01bde6a94c0d16b26b20d1ba30e69bec0457972e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812534"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="c8c2d-103">Tipo de recurso mobileApp</span><span class="sxs-lookup"><span data-stu-id="c8c2d-103">mobileApp resource type</span></span>

> <span data-ttu-id="c8c2d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8c2d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8c2d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8c2d-107">Uma classe abstrata que contém as propriedades base de aplicativos móveis do Intune.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-107">An abstract class containing the base properties for Intune mobile apps.</span></span>
## <a name="methods"></a><span data-ttu-id="c8c2d-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="c8c2d-108">Methods</span></span>
|<span data-ttu-id="c8c2d-109">Método</span><span class="sxs-lookup"><span data-stu-id="c8c2d-109">Method</span></span>|<span data-ttu-id="c8c2d-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c8c2d-110">Return Type</span></span>|<span data-ttu-id="c8c2d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8c2d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c8c2d-112">Listar mobileApps</span><span class="sxs-lookup"><span data-stu-id="c8c2d-112">List mobileApps</span></span>](../api/intune-apps-mobileapp-list.md)|<span data-ttu-id="c8c2d-113">Coleção [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c8c2d-113">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="c8c2d-114">Lista propriedades e relações dos objetos [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c8c2d-114">List properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="c8c2d-115">Obter mobileApp</span><span class="sxs-lookup"><span data-stu-id="c8c2d-115">Get mobileApp</span></span>](../api/intune-apps-mobileapp-get.md)|[<span data-ttu-id="c8c2d-116">mobileApp</span><span class="sxs-lookup"><span data-stu-id="c8c2d-116">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="c8c2d-117">Propriedades de leitura e relações do objeto [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c8c2d-117">Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.</span></span>|
|[<span data-ttu-id="c8c2d-118">ação assign</span><span class="sxs-lookup"><span data-stu-id="c8c2d-118">assign action</span></span>](../api/intune-apps-mobileapp-assign.md)|<span data-ttu-id="c8c2d-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c8c2d-119">None</span></span>|<span data-ttu-id="c8c2d-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c8c2d-120">Not yet documented</span></span>|
|[<span data-ttu-id="c8c2d-121">função getMobileAppCount</span><span class="sxs-lookup"><span data-stu-id="c8c2d-121">getMobileAppCount function</span></span>](../api/intune-apps-mobileapp-getmobileappcount.md)|<span data-ttu-id="c8c2d-122">Int64</span><span class="sxs-lookup"><span data-stu-id="c8c2d-122">Int64</span></span>|<span data-ttu-id="c8c2d-123">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c8c2d-123">Not yet documented</span></span>|
|[<span data-ttu-id="c8c2d-124">função getTopMobileApps</span><span class="sxs-lookup"><span data-stu-id="c8c2d-124">getTopMobileApps function</span></span>](../api/intune-apps-mobileapp-gettopmobileapps.md)|<span data-ttu-id="c8c2d-125">Coleção [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c8c2d-125">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="c8c2d-126">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c8c2d-126">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c8c2d-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c8c2d-127">Properties</span></span>
|<span data-ttu-id="c8c2d-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8c2d-128">Property</span></span>|<span data-ttu-id="c8c2d-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8c2d-129">Type</span></span>|<span data-ttu-id="c8c2d-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8c2d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8c2d-131">id</span><span class="sxs-lookup"><span data-stu-id="c8c2d-131">id</span></span>|<span data-ttu-id="c8c2d-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8c2d-132">String</span></span>|<span data-ttu-id="c8c2d-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-133">Key of the entity.</span></span>|
|<span data-ttu-id="c8c2d-134">displayName</span><span class="sxs-lookup"><span data-stu-id="c8c2d-134">displayName</span></span>|<span data-ttu-id="c8c2d-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8c2d-135">String</span></span>|<span data-ttu-id="c8c2d-136">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-136">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="c8c2d-137">description</span><span class="sxs-lookup"><span data-stu-id="c8c2d-137">description</span></span>|<span data-ttu-id="c8c2d-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8c2d-138">String</span></span>|<span data-ttu-id="c8c2d-139">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-139">The description of the app.</span></span>|
|<span data-ttu-id="c8c2d-140">publisher</span><span class="sxs-lookup"><span data-stu-id="c8c2d-140">publisher</span></span>|<span data-ttu-id="c8c2d-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8c2d-141">String</span></span>|<span data-ttu-id="c8c2d-142">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-142">The publisher of the app.</span></span>|
|<span data-ttu-id="c8c2d-143">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c8c2d-143">largeIcon</span></span>|[<span data-ttu-id="c8c2d-144">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c8c2d-144">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c8c2d-145">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-145">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="c8c2d-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c8c2d-146">createdDateTime</span></span>|<span data-ttu-id="c8c2d-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8c2d-147">DateTimeOffset</span></span>|<span data-ttu-id="c8c2d-148">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-148">The date and time the app was created.</span></span>|
|<span data-ttu-id="c8c2d-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8c2d-149">lastModifiedDateTime</span></span>|<span data-ttu-id="c8c2d-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8c2d-150">DateTimeOffset</span></span>|<span data-ttu-id="c8c2d-151">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-151">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="c8c2d-152">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c8c2d-152">isFeatured</span></span>|<span data-ttu-id="c8c2d-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="c8c2d-153">Boolean</span></span>|<span data-ttu-id="c8c2d-154">O valor que indica se o aplicativo está marcado como em destaque pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-154">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="c8c2d-155">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c8c2d-155">privacyInformationUrl</span></span>|<span data-ttu-id="c8c2d-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8c2d-156">String</span></span>|<span data-ttu-id="c8c2d-157">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-157">The privacy statement Url.</span></span>|
|<span data-ttu-id="c8c2d-158">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c8c2d-158">informationUrl</span></span>|<span data-ttu-id="c8c2d-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8c2d-159">String</span></span>|<span data-ttu-id="c8c2d-160">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-160">The more information Url.</span></span>|
|<span data-ttu-id="c8c2d-161">owner</span><span class="sxs-lookup"><span data-stu-id="c8c2d-161">owner</span></span>|<span data-ttu-id="c8c2d-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8c2d-162">String</span></span>|<span data-ttu-id="c8c2d-163">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-163">The owner of the app.</span></span>|
|<span data-ttu-id="c8c2d-164">developer</span><span class="sxs-lookup"><span data-stu-id="c8c2d-164">developer</span></span>|<span data-ttu-id="c8c2d-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8c2d-165">String</span></span>|<span data-ttu-id="c8c2d-166">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-166">The developer of the app.</span></span>|
|<span data-ttu-id="c8c2d-167">notes</span><span class="sxs-lookup"><span data-stu-id="c8c2d-167">notes</span></span>|<span data-ttu-id="c8c2d-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8c2d-168">String</span></span>|<span data-ttu-id="c8c2d-169">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-169">Notes for the app.</span></span>|
|<span data-ttu-id="c8c2d-170">uploadState</span><span class="sxs-lookup"><span data-stu-id="c8c2d-170">uploadState</span></span>|<span data-ttu-id="c8c2d-171">Int32</span><span class="sxs-lookup"><span data-stu-id="c8c2d-171">Int32</span></span>|<span data-ttu-id="c8c2d-172">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-172">The upload state.</span></span>|
|<span data-ttu-id="c8c2d-173">publishingState</span><span class="sxs-lookup"><span data-stu-id="c8c2d-173">publishingState</span></span>|[<span data-ttu-id="c8c2d-174">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c8c2d-174">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c8c2d-175">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-175">The publishing state for the app.</span></span> <span data-ttu-id="c8c2d-176">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-176">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c8c2d-177">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-177">Possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8c2d-178">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="c8c2d-178">Relationships</span></span>
|<span data-ttu-id="c8c2d-179">Relação</span><span class="sxs-lookup"><span data-stu-id="c8c2d-179">Relationship</span></span>|<span data-ttu-id="c8c2d-180">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8c2d-180">Type</span></span>|<span data-ttu-id="c8c2d-181">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8c2d-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8c2d-182">categories</span><span class="sxs-lookup"><span data-stu-id="c8c2d-182">categories</span></span>|<span data-ttu-id="c8c2d-183">Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="c8c2d-183">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="c8c2d-184">A lista de categorias para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-184">The list of categories for this app.</span></span>|
|<span data-ttu-id="c8c2d-185">assignments</span><span class="sxs-lookup"><span data-stu-id="c8c2d-185">assignments</span></span>|<span data-ttu-id="c8c2d-186">Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c8c2d-186">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="c8c2d-187">A lista de atribuições de grupo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-187">The list of group assignments for this mobile app.</span></span>|
|<span data-ttu-id="c8c2d-188">installSummary</span><span class="sxs-lookup"><span data-stu-id="c8c2d-188">installSummary</span></span>|[<span data-ttu-id="c8c2d-189">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="c8c2d-189">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="c8c2d-190">Resumo de instalação do aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-190">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="c8c2d-191">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="c8c2d-191">deviceStatuses</span></span>|<span data-ttu-id="c8c2d-192">coleção [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="c8c2d-192">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="c8c2d-193">A lista de estados de instalação para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-193">The list of installation states for this mobile app.</span></span>|
|<span data-ttu-id="c8c2d-194">userStatuses</span><span class="sxs-lookup"><span data-stu-id="c8c2d-194">userStatuses</span></span>|<span data-ttu-id="c8c2d-195">coleção [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="c8c2d-195">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="c8c2d-196">A lista de estados de instalação para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-196">The list of installation states for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c8c2d-197">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c8c2d-197">JSON Representation</span></span>
<span data-ttu-id="c8c2d-198">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c8c2d-198">Here is a JSON representation of the resource.</span></span>
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
  "publishingState": "String"
}
```





