---
title: Tipo de recurso mobileLobApp
description: Uma classe base abstrata que contém propriedades para a toda a linha móvel de aplicativos de negócios.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3814ac40f52ff65e4e884923539b14f24f3fb4d0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094306"
---
# <a name="mobilelobapp-resource-type"></a><span data-ttu-id="e532a-103">Tipo de recurso mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="e532a-103">mobileLobApp resource type</span></span>

<span data-ttu-id="e532a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e532a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e532a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e532a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e532a-106">Uma classe base abstrata que contém propriedades para a toda a linha móvel de aplicativos de negócios.</span><span class="sxs-lookup"><span data-stu-id="e532a-106">An abstract base class containing properties for all mobile line of business apps.</span></span>


<span data-ttu-id="e532a-107">Herda de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e532a-107">Inherits from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="e532a-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="e532a-108">Methods</span></span>
|<span data-ttu-id="e532a-109">Método</span><span class="sxs-lookup"><span data-stu-id="e532a-109">Method</span></span>|<span data-ttu-id="e532a-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e532a-110">Return Type</span></span>|<span data-ttu-id="e532a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e532a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e532a-112">Listar mobileLobApps</span><span class="sxs-lookup"><span data-stu-id="e532a-112">List mobileLobApps</span></span>](../api/intune-apps-mobilelobapp-list.md)|<span data-ttu-id="e532a-113">Coleção [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e532a-113">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) collection</span></span>|<span data-ttu-id="e532a-114">Lista propriedades e relações dos objetos [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e532a-114">List properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) objects.</span></span>|
|[<span data-ttu-id="e532a-115">Obter mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="e532a-115">Get mobileLobApp</span></span>](../api/intune-apps-mobilelobapp-get.md)|[<span data-ttu-id="e532a-116">mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="e532a-116">mobileLobApp</span></span>](../resources/intune-apps-mobilelobapp.md)|<span data-ttu-id="e532a-117">Propriedades de leitura e relações do objeto [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e532a-117">Read properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e532a-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e532a-118">Properties</span></span>
|<span data-ttu-id="e532a-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e532a-119">Property</span></span>|<span data-ttu-id="e532a-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="e532a-120">Type</span></span>|<span data-ttu-id="e532a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e532a-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e532a-122">id</span><span class="sxs-lookup"><span data-stu-id="e532a-122">id</span></span>|<span data-ttu-id="e532a-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e532a-123">String</span></span>|<span data-ttu-id="e532a-124">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e532a-124">Key of the entity.</span></span> <span data-ttu-id="e532a-125">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e532a-125">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e532a-126">displayName</span><span class="sxs-lookup"><span data-stu-id="e532a-126">displayName</span></span>|<span data-ttu-id="e532a-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e532a-127">String</span></span>|<span data-ttu-id="e532a-128">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="e532a-128">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e532a-129">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e532a-129">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e532a-130">description</span><span class="sxs-lookup"><span data-stu-id="e532a-130">description</span></span>|<span data-ttu-id="e532a-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e532a-131">String</span></span>|<span data-ttu-id="e532a-132">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e532a-132">The description of the app.</span></span> <span data-ttu-id="e532a-133">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e532a-133">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e532a-134">publicador</span><span class="sxs-lookup"><span data-stu-id="e532a-134">publisher</span></span>|<span data-ttu-id="e532a-135">String</span><span class="sxs-lookup"><span data-stu-id="e532a-135">String</span></span>|<span data-ttu-id="e532a-136">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e532a-136">The publisher of the app.</span></span> <span data-ttu-id="e532a-137">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e532a-137">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e532a-138">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e532a-138">largeIcon</span></span>|[<span data-ttu-id="e532a-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e532a-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e532a-140">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="e532a-140">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e532a-141">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e532a-141">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e532a-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e532a-142">createdDateTime</span></span>|<span data-ttu-id="e532a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e532a-143">DateTimeOffset</span></span>|<span data-ttu-id="e532a-144">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e532a-144">The date and time the app was created.</span></span> <span data-ttu-id="e532a-145">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e532a-145">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e532a-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e532a-146">lastModifiedDateTime</span></span>|<span data-ttu-id="e532a-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e532a-147">DateTimeOffset</span></span>|<span data-ttu-id="e532a-148">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e532a-148">The date and time the app was last modified.</span></span> <span data-ttu-id="e532a-149">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e532a-149">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e532a-150">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e532a-150">isFeatured</span></span>|<span data-ttu-id="e532a-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="e532a-151">Boolean</span></span>|<span data-ttu-id="e532a-152">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e532a-152">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e532a-153">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e532a-153">privacyInformationUrl</span></span>|<span data-ttu-id="e532a-154">String</span><span class="sxs-lookup"><span data-stu-id="e532a-154">String</span></span>|<span data-ttu-id="e532a-155">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="e532a-155">The privacy statement Url.</span></span> <span data-ttu-id="e532a-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e532a-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e532a-157">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e532a-157">informationUrl</span></span>|<span data-ttu-id="e532a-158">String</span><span class="sxs-lookup"><span data-stu-id="e532a-158">String</span></span>|<span data-ttu-id="e532a-159">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="e532a-159">The more information Url.</span></span> <span data-ttu-id="e532a-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e532a-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e532a-161">owner</span><span class="sxs-lookup"><span data-stu-id="e532a-161">owner</span></span>|<span data-ttu-id="e532a-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e532a-162">String</span></span>|<span data-ttu-id="e532a-163">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e532a-163">The owner of the app.</span></span> <span data-ttu-id="e532a-164">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e532a-164">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e532a-165">developer</span><span class="sxs-lookup"><span data-stu-id="e532a-165">developer</span></span>|<span data-ttu-id="e532a-166">String</span><span class="sxs-lookup"><span data-stu-id="e532a-166">String</span></span>|<span data-ttu-id="e532a-167">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e532a-167">The developer of the app.</span></span> <span data-ttu-id="e532a-168">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e532a-168">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e532a-169">notes</span><span class="sxs-lookup"><span data-stu-id="e532a-169">notes</span></span>|<span data-ttu-id="e532a-170">String</span><span class="sxs-lookup"><span data-stu-id="e532a-170">String</span></span>|<span data-ttu-id="e532a-171">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e532a-171">Notes for the app.</span></span> <span data-ttu-id="e532a-172">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e532a-172">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e532a-173">publishingState</span><span class="sxs-lookup"><span data-stu-id="e532a-173">publishingState</span></span>|[<span data-ttu-id="e532a-174">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e532a-174">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e532a-175">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e532a-175">The publishing state for the app.</span></span> <span data-ttu-id="e532a-176">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="e532a-176">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e532a-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e532a-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e532a-178">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e532a-178">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e532a-179">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e532a-179">committedContentVersion</span></span>|<span data-ttu-id="e532a-180">String</span><span class="sxs-lookup"><span data-stu-id="e532a-180">String</span></span>|<span data-ttu-id="e532a-181">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="e532a-181">The internal committed content version.</span></span>|
|<span data-ttu-id="e532a-182">fileName</span><span class="sxs-lookup"><span data-stu-id="e532a-182">fileName</span></span>|<span data-ttu-id="e532a-183">String</span><span class="sxs-lookup"><span data-stu-id="e532a-183">String</span></span>|<span data-ttu-id="e532a-184">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="e532a-184">The name of the main Lob application file.</span></span>|
|<span data-ttu-id="e532a-185">size</span><span class="sxs-lookup"><span data-stu-id="e532a-185">size</span></span>|<span data-ttu-id="e532a-186">Int64</span><span class="sxs-lookup"><span data-stu-id="e532a-186">Int64</span></span>|<span data-ttu-id="e532a-187">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="e532a-187">The total size, including all uploaded files.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e532a-188">Relações</span><span class="sxs-lookup"><span data-stu-id="e532a-188">Relationships</span></span>
|<span data-ttu-id="e532a-189">Relação</span><span class="sxs-lookup"><span data-stu-id="e532a-189">Relationship</span></span>|<span data-ttu-id="e532a-190">Tipo</span><span class="sxs-lookup"><span data-stu-id="e532a-190">Type</span></span>|<span data-ttu-id="e532a-191">Descrição</span><span class="sxs-lookup"><span data-stu-id="e532a-191">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e532a-192">categories</span><span class="sxs-lookup"><span data-stu-id="e532a-192">categories</span></span>|<span data-ttu-id="e532a-193">Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="e532a-193">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="e532a-194">A lista de categorias para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e532a-194">The list of categories for this app.</span></span> <span data-ttu-id="e532a-195">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e532a-195">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e532a-196">assignments</span><span class="sxs-lookup"><span data-stu-id="e532a-196">assignments</span></span>|<span data-ttu-id="e532a-197">Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e532a-197">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="e532a-198">A lista de atribuições de grupo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="e532a-198">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="e532a-199">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e532a-199">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e532a-200">contentVersions</span><span class="sxs-lookup"><span data-stu-id="e532a-200">contentVersions</span></span>|<span data-ttu-id="e532a-201">Coleção [mobileAppContent](../resources/intune-apps-mobileappcontent.md)</span><span class="sxs-lookup"><span data-stu-id="e532a-201">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="e532a-202">A lista das versões de conteúdo deste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e532a-202">The list of content versions for this app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e532a-203">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e532a-203">JSON Representation</span></span>
<span data-ttu-id="e532a-204">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e532a-204">Here is a JSON representation of the resource.</span></span>
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









