---
title: Tipo de recurso managedApp
description: Classe abstrata que contém propriedades e propriedades herdadas para aplicativos que você pode gerenciar com uma política de proteção de aplicativos do Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4fbb934f3bb52c1980908c1595c2252800c465e3
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756047"
---
# <a name="managedapp-resource-type"></a><span data-ttu-id="b0b46-103">Tipo de recurso managedApp</span><span class="sxs-lookup"><span data-stu-id="b0b46-103">managedApp resource type</span></span>

<span data-ttu-id="b0b46-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0b46-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0b46-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0b46-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0b46-106">Classe abstrata que contém propriedades e propriedades herdadas para aplicativos que você pode gerenciar com uma política de proteção de aplicativos do Intune.</span><span class="sxs-lookup"><span data-stu-id="b0b46-106">Abstract class that contains properties and inherited properties for apps that you can manage with an Intune app protection policy.</span></span>


<span data-ttu-id="b0b46-107">Herda de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0b46-107">Inherits from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="b0b46-108">Methods</span><span class="sxs-lookup"><span data-stu-id="b0b46-108">Methods</span></span>
|<span data-ttu-id="b0b46-109">Método</span><span class="sxs-lookup"><span data-stu-id="b0b46-109">Method</span></span>|<span data-ttu-id="b0b46-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b0b46-110">Return Type</span></span>|<span data-ttu-id="b0b46-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0b46-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b0b46-112">Listar managedApps</span><span class="sxs-lookup"><span data-stu-id="b0b46-112">List managedApps</span></span>](../api/intune-apps-managedapp-list.md)|<span data-ttu-id="b0b46-113">Coleção [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0b46-113">[managedApp](../resources/intune-apps-managedapp.md) collection</span></span>|<span data-ttu-id="b0b46-114">Lista propriedades e relações dos objetos [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="b0b46-114">List properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) objects.</span></span>|
|[<span data-ttu-id="b0b46-115">Obter managedApp</span><span class="sxs-lookup"><span data-stu-id="b0b46-115">Get managedApp</span></span>](../api/intune-apps-managedapp-get.md)|[<span data-ttu-id="b0b46-116">managedApp</span><span class="sxs-lookup"><span data-stu-id="b0b46-116">managedApp</span></span>](../resources/intune-apps-managedapp.md)|<span data-ttu-id="b0b46-117">Propriedades de leitura e relações do objeto [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="b0b46-117">Read properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b0b46-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0b46-118">Properties</span></span>
|<span data-ttu-id="b0b46-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0b46-119">Property</span></span>|<span data-ttu-id="b0b46-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0b46-120">Type</span></span>|<span data-ttu-id="b0b46-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0b46-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0b46-122">id</span><span class="sxs-lookup"><span data-stu-id="b0b46-122">id</span></span>|<span data-ttu-id="b0b46-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0b46-123">String</span></span>|<span data-ttu-id="b0b46-124">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b0b46-124">Key of the entity.</span></span> <span data-ttu-id="b0b46-125">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0b46-125">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0b46-126">displayName</span><span class="sxs-lookup"><span data-stu-id="b0b46-126">displayName</span></span>|<span data-ttu-id="b0b46-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0b46-127">String</span></span>|<span data-ttu-id="b0b46-128">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="b0b46-128">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b0b46-129">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0b46-129">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0b46-130">descrição</span><span class="sxs-lookup"><span data-stu-id="b0b46-130">description</span></span>|<span data-ttu-id="b0b46-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0b46-131">String</span></span>|<span data-ttu-id="b0b46-132">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b0b46-132">The description of the app.</span></span> <span data-ttu-id="b0b46-133">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0b46-133">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0b46-134">publicador</span><span class="sxs-lookup"><span data-stu-id="b0b46-134">publisher</span></span>|<span data-ttu-id="b0b46-135">String</span><span class="sxs-lookup"><span data-stu-id="b0b46-135">String</span></span>|<span data-ttu-id="b0b46-136">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b0b46-136">The publisher of the app.</span></span> <span data-ttu-id="b0b46-137">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0b46-137">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0b46-138">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b0b46-138">largeIcon</span></span>|[<span data-ttu-id="b0b46-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b0b46-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b0b46-140">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="b0b46-140">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b0b46-141">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0b46-141">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0b46-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b0b46-142">createdDateTime</span></span>|<span data-ttu-id="b0b46-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0b46-143">DateTimeOffset</span></span>|<span data-ttu-id="b0b46-144">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b0b46-144">The date and time the app was created.</span></span> <span data-ttu-id="b0b46-145">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0b46-145">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0b46-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0b46-146">lastModifiedDateTime</span></span>|<span data-ttu-id="b0b46-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0b46-147">DateTimeOffset</span></span>|<span data-ttu-id="b0b46-148">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b0b46-148">The date and time the app was last modified.</span></span> <span data-ttu-id="b0b46-149">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0b46-149">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0b46-150">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b0b46-150">isFeatured</span></span>|<span data-ttu-id="b0b46-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0b46-151">Boolean</span></span>|<span data-ttu-id="b0b46-152">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0b46-152">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0b46-153">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b0b46-153">privacyInformationUrl</span></span>|<span data-ttu-id="b0b46-154">String</span><span class="sxs-lookup"><span data-stu-id="b0b46-154">String</span></span>|<span data-ttu-id="b0b46-155">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="b0b46-155">The privacy statement Url.</span></span> <span data-ttu-id="b0b46-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0b46-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0b46-157">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b0b46-157">informationUrl</span></span>|<span data-ttu-id="b0b46-158">String</span><span class="sxs-lookup"><span data-stu-id="b0b46-158">String</span></span>|<span data-ttu-id="b0b46-159">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="b0b46-159">The more information Url.</span></span> <span data-ttu-id="b0b46-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0b46-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0b46-161">proprietário</span><span class="sxs-lookup"><span data-stu-id="b0b46-161">owner</span></span>|<span data-ttu-id="b0b46-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0b46-162">String</span></span>|<span data-ttu-id="b0b46-163">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="b0b46-163">The owner of the app.</span></span> <span data-ttu-id="b0b46-164">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0b46-164">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0b46-165">developer</span><span class="sxs-lookup"><span data-stu-id="b0b46-165">developer</span></span>|<span data-ttu-id="b0b46-166">String</span><span class="sxs-lookup"><span data-stu-id="b0b46-166">String</span></span>|<span data-ttu-id="b0b46-167">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b0b46-167">The developer of the app.</span></span> <span data-ttu-id="b0b46-168">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0b46-168">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0b46-169">notes</span><span class="sxs-lookup"><span data-stu-id="b0b46-169">notes</span></span>|<span data-ttu-id="b0b46-170">String</span><span class="sxs-lookup"><span data-stu-id="b0b46-170">String</span></span>|<span data-ttu-id="b0b46-171">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b0b46-171">Notes for the app.</span></span> <span data-ttu-id="b0b46-172">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0b46-172">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0b46-173">publishingState</span><span class="sxs-lookup"><span data-stu-id="b0b46-173">publishingState</span></span>|[<span data-ttu-id="b0b46-174">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b0b46-174">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b0b46-175">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b0b46-175">The publishing state for the app.</span></span> <span data-ttu-id="b0b46-176">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="b0b46-176">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b0b46-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b0b46-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b0b46-178">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b0b46-178">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b0b46-179">appAvailability</span><span class="sxs-lookup"><span data-stu-id="b0b46-179">appAvailability</span></span>|[<span data-ttu-id="b0b46-180">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="b0b46-180">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="b0b46-181">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b0b46-181">The Application's availability.</span></span> <span data-ttu-id="b0b46-182">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="b0b46-182">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="b0b46-183">version</span><span class="sxs-lookup"><span data-stu-id="b0b46-183">version</span></span>|<span data-ttu-id="b0b46-184">String</span><span class="sxs-lookup"><span data-stu-id="b0b46-184">String</span></span>|<span data-ttu-id="b0b46-185">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b0b46-185">The Application's version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0b46-186">Relações</span><span class="sxs-lookup"><span data-stu-id="b0b46-186">Relationships</span></span>
|<span data-ttu-id="b0b46-187">Relação</span><span class="sxs-lookup"><span data-stu-id="b0b46-187">Relationship</span></span>|<span data-ttu-id="b0b46-188">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0b46-188">Type</span></span>|<span data-ttu-id="b0b46-189">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0b46-189">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0b46-190">categories</span><span class="sxs-lookup"><span data-stu-id="b0b46-190">categories</span></span>|<span data-ttu-id="b0b46-191">Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="b0b46-191">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="b0b46-192">A lista de categorias para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b0b46-192">The list of categories for this app.</span></span> <span data-ttu-id="b0b46-193">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0b46-193">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b0b46-194">assignments</span><span class="sxs-lookup"><span data-stu-id="b0b46-194">assignments</span></span>|<span data-ttu-id="b0b46-195">Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b0b46-195">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="b0b46-196">A lista de atribuições de grupo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="b0b46-196">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="b0b46-197">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0b46-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b0b46-198">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0b46-198">JSON Representation</span></span>
<span data-ttu-id="b0b46-199">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0b46-199">Here is a JSON representation of the resource.</span></span>
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




