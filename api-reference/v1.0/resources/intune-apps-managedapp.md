---
title: Tipo de recurso managedApp
description: Classe abstrata que contém propriedades e propriedades herdadas para aplicativos que você pode gerenciar com uma política de proteção de aplicativos do Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 72cb905c266dba33c635dded929b32bc333705f4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015413"
---
# <a name="managedapp-resource-type"></a><span data-ttu-id="f6ca2-103">Tipo de recurso managedApp</span><span class="sxs-lookup"><span data-stu-id="f6ca2-103">managedApp resource type</span></span>

<span data-ttu-id="f6ca2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6ca2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6ca2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f6ca2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6ca2-106">Classe abstrata que contém propriedades e propriedades herdadas para aplicativos que você pode gerenciar com uma política de proteção de aplicativos do Intune.</span><span class="sxs-lookup"><span data-stu-id="f6ca2-106">Abstract class that contains properties and inherited properties for apps that you can manage with an Intune app protection policy.</span></span>


<span data-ttu-id="f6ca2-107">Herda de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f6ca2-107">Inherits from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="f6ca2-108">Methods</span><span class="sxs-lookup"><span data-stu-id="f6ca2-108">Methods</span></span>
|<span data-ttu-id="f6ca2-109">Método</span><span class="sxs-lookup"><span data-stu-id="f6ca2-109">Method</span></span>|<span data-ttu-id="f6ca2-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f6ca2-110">Return Type</span></span>|<span data-ttu-id="f6ca2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6ca2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f6ca2-112">Listar managedApps</span><span class="sxs-lookup"><span data-stu-id="f6ca2-112">List managedApps</span></span>](../api/intune-apps-managedapp-list.md)|<span data-ttu-id="f6ca2-113">Coleção [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="f6ca2-113">[managedApp](../resources/intune-apps-managedapp.md) collection</span></span>|<span data-ttu-id="f6ca2-114">Lista propriedades e relações dos objetos [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="f6ca2-114">List properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) objects.</span></span>|
|[<span data-ttu-id="f6ca2-115">Obter managedApp</span><span class="sxs-lookup"><span data-stu-id="f6ca2-115">Get managedApp</span></span>](../api/intune-apps-managedapp-get.md)|[<span data-ttu-id="f6ca2-116">managedApp</span><span class="sxs-lookup"><span data-stu-id="f6ca2-116">managedApp</span></span>](../resources/intune-apps-managedapp.md)|<span data-ttu-id="f6ca2-117">Propriedades de leitura e relações do objeto [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="f6ca2-117">Read properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f6ca2-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f6ca2-118">Properties</span></span>
|<span data-ttu-id="f6ca2-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f6ca2-119">Property</span></span>|<span data-ttu-id="f6ca2-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6ca2-120">Type</span></span>|<span data-ttu-id="f6ca2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6ca2-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6ca2-122">id</span><span class="sxs-lookup"><span data-stu-id="f6ca2-122">id</span></span>|<span data-ttu-id="f6ca2-123">String</span><span class="sxs-lookup"><span data-stu-id="f6ca2-123">String</span></span>|<span data-ttu-id="f6ca2-124">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f6ca2-124">Key of the entity.</span></span> <span data-ttu-id="f6ca2-125">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f6ca2-125">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ca2-126">displayName</span><span class="sxs-lookup"><span data-stu-id="f6ca2-126">displayName</span></span>|<span data-ttu-id="f6ca2-127">String</span><span class="sxs-lookup"><span data-stu-id="f6ca2-127">String</span></span>|<span data-ttu-id="f6ca2-128">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="f6ca2-128">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f6ca2-129">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f6ca2-129">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ca2-130">description</span><span class="sxs-lookup"><span data-stu-id="f6ca2-130">description</span></span>|<span data-ttu-id="f6ca2-131">String</span><span class="sxs-lookup"><span data-stu-id="f6ca2-131">String</span></span>|<span data-ttu-id="f6ca2-132">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f6ca2-132">The description of the app.</span></span> <span data-ttu-id="f6ca2-133">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f6ca2-133">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ca2-134">publicador</span><span class="sxs-lookup"><span data-stu-id="f6ca2-134">publisher</span></span>|<span data-ttu-id="f6ca2-135">String</span><span class="sxs-lookup"><span data-stu-id="f6ca2-135">String</span></span>|<span data-ttu-id="f6ca2-136">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f6ca2-136">The publisher of the app.</span></span> <span data-ttu-id="f6ca2-137">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f6ca2-137">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ca2-138">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f6ca2-138">largeIcon</span></span>|[<span data-ttu-id="f6ca2-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f6ca2-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f6ca2-140">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="f6ca2-140">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f6ca2-141">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f6ca2-141">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ca2-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f6ca2-142">createdDateTime</span></span>|<span data-ttu-id="f6ca2-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6ca2-143">DateTimeOffset</span></span>|<span data-ttu-id="f6ca2-144">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f6ca2-144">The date and time the app was created.</span></span> <span data-ttu-id="f6ca2-145">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f6ca2-145">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ca2-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6ca2-146">lastModifiedDateTime</span></span>|<span data-ttu-id="f6ca2-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6ca2-147">DateTimeOffset</span></span>|<span data-ttu-id="f6ca2-148">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f6ca2-148">The date and time the app was last modified.</span></span> <span data-ttu-id="f6ca2-149">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f6ca2-149">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ca2-150">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f6ca2-150">isFeatured</span></span>|<span data-ttu-id="f6ca2-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6ca2-151">Boolean</span></span>|<span data-ttu-id="f6ca2-152">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f6ca2-152">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ca2-153">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f6ca2-153">privacyInformationUrl</span></span>|<span data-ttu-id="f6ca2-154">String</span><span class="sxs-lookup"><span data-stu-id="f6ca2-154">String</span></span>|<span data-ttu-id="f6ca2-155">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="f6ca2-155">The privacy statement Url.</span></span> <span data-ttu-id="f6ca2-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f6ca2-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ca2-157">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f6ca2-157">informationUrl</span></span>|<span data-ttu-id="f6ca2-158">String</span><span class="sxs-lookup"><span data-stu-id="f6ca2-158">String</span></span>|<span data-ttu-id="f6ca2-159">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="f6ca2-159">The more information Url.</span></span> <span data-ttu-id="f6ca2-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f6ca2-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ca2-161">proprietário</span><span class="sxs-lookup"><span data-stu-id="f6ca2-161">owner</span></span>|<span data-ttu-id="f6ca2-162">String</span><span class="sxs-lookup"><span data-stu-id="f6ca2-162">String</span></span>|<span data-ttu-id="f6ca2-163">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f6ca2-163">The owner of the app.</span></span> <span data-ttu-id="f6ca2-164">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f6ca2-164">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ca2-165">developer</span><span class="sxs-lookup"><span data-stu-id="f6ca2-165">developer</span></span>|<span data-ttu-id="f6ca2-166">String</span><span class="sxs-lookup"><span data-stu-id="f6ca2-166">String</span></span>|<span data-ttu-id="f6ca2-167">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f6ca2-167">The developer of the app.</span></span> <span data-ttu-id="f6ca2-168">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f6ca2-168">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ca2-169">notes</span><span class="sxs-lookup"><span data-stu-id="f6ca2-169">notes</span></span>|<span data-ttu-id="f6ca2-170">String</span><span class="sxs-lookup"><span data-stu-id="f6ca2-170">String</span></span>|<span data-ttu-id="f6ca2-171">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f6ca2-171">Notes for the app.</span></span> <span data-ttu-id="f6ca2-172">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f6ca2-172">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ca2-173">publishingState</span><span class="sxs-lookup"><span data-stu-id="f6ca2-173">publishingState</span></span>|[<span data-ttu-id="f6ca2-174">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f6ca2-174">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f6ca2-175">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f6ca2-175">The publishing state for the app.</span></span> <span data-ttu-id="f6ca2-176">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="f6ca2-176">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f6ca2-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f6ca2-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f6ca2-178">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f6ca2-178">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f6ca2-179">appAvailability</span><span class="sxs-lookup"><span data-stu-id="f6ca2-179">appAvailability</span></span>|[<span data-ttu-id="f6ca2-180">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="f6ca2-180">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="f6ca2-181">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f6ca2-181">The Application's availability.</span></span> <span data-ttu-id="f6ca2-182">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="f6ca2-182">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="f6ca2-183">version</span><span class="sxs-lookup"><span data-stu-id="f6ca2-183">version</span></span>|<span data-ttu-id="f6ca2-184">String</span><span class="sxs-lookup"><span data-stu-id="f6ca2-184">String</span></span>|<span data-ttu-id="f6ca2-185">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f6ca2-185">The Application's version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6ca2-186">Relações</span><span class="sxs-lookup"><span data-stu-id="f6ca2-186">Relationships</span></span>
|<span data-ttu-id="f6ca2-187">Relação</span><span class="sxs-lookup"><span data-stu-id="f6ca2-187">Relationship</span></span>|<span data-ttu-id="f6ca2-188">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6ca2-188">Type</span></span>|<span data-ttu-id="f6ca2-189">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6ca2-189">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6ca2-190">categories</span><span class="sxs-lookup"><span data-stu-id="f6ca2-190">categories</span></span>|<span data-ttu-id="f6ca2-191">Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="f6ca2-191">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="f6ca2-192">A lista de categorias para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f6ca2-192">The list of categories for this app.</span></span> <span data-ttu-id="f6ca2-193">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f6ca2-193">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f6ca2-194">assignments</span><span class="sxs-lookup"><span data-stu-id="f6ca2-194">assignments</span></span>|<span data-ttu-id="f6ca2-195">Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f6ca2-195">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="f6ca2-196">A lista de atribuições de grupo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="f6ca2-196">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="f6ca2-197">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f6ca2-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f6ca2-198">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f6ca2-198">JSON Representation</span></span>
<span data-ttu-id="f6ca2-199">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f6ca2-199">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedApp",
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
  "appAvailability": "String",
  "version": "String"
}
```









