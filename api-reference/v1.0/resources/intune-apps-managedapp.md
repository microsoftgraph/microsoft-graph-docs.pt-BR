---
title: Tipo de recurso managedApp
description: Classe abstrata que contém propriedades e propriedades herdadas para aplicativos que você pode gerenciar com uma política de proteção de aplicativos do Intune.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 48383aa528e0102dd8c1a77f22edd41d0385a8e6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532787"
---
# <a name="managedapp-resource-type"></a><span data-ttu-id="780eb-103">Tipo de recurso managedApp</span><span class="sxs-lookup"><span data-stu-id="780eb-103">managedApp resource type</span></span>

<span data-ttu-id="780eb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="780eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="780eb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="780eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="780eb-106">Classe abstrata que contém propriedades e propriedades herdadas para aplicativos que você pode gerenciar com uma política de proteção de aplicativos do Intune.</span><span class="sxs-lookup"><span data-stu-id="780eb-106">Abstract class that contains properties and inherited properties for apps that you can manage with an Intune app protection policy.</span></span>


<span data-ttu-id="780eb-107">Herda de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="780eb-107">Inherits from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="780eb-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="780eb-108">Methods</span></span>
|<span data-ttu-id="780eb-109">Método</span><span class="sxs-lookup"><span data-stu-id="780eb-109">Method</span></span>|<span data-ttu-id="780eb-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="780eb-110">Return Type</span></span>|<span data-ttu-id="780eb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="780eb-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="780eb-112">Listar managedApps</span><span class="sxs-lookup"><span data-stu-id="780eb-112">List managedApps</span></span>](../api/intune-apps-managedapp-list.md)|<span data-ttu-id="780eb-113">Coleção [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="780eb-113">[managedApp](../resources/intune-apps-managedapp.md) collection</span></span>|<span data-ttu-id="780eb-114">Lista propriedades e relações dos objetos [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="780eb-114">List properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) objects.</span></span>|
|[<span data-ttu-id="780eb-115">Obter managedApp</span><span class="sxs-lookup"><span data-stu-id="780eb-115">Get managedApp</span></span>](../api/intune-apps-managedapp-get.md)|[<span data-ttu-id="780eb-116">managedApp</span><span class="sxs-lookup"><span data-stu-id="780eb-116">managedApp</span></span>](../resources/intune-apps-managedapp.md)|<span data-ttu-id="780eb-117">Propriedades de leitura e relações do objeto [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="780eb-117">Read properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="780eb-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="780eb-118">Properties</span></span>
|<span data-ttu-id="780eb-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="780eb-119">Property</span></span>|<span data-ttu-id="780eb-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="780eb-120">Type</span></span>|<span data-ttu-id="780eb-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="780eb-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="780eb-122">id</span><span class="sxs-lookup"><span data-stu-id="780eb-122">id</span></span>|<span data-ttu-id="780eb-123">String</span><span class="sxs-lookup"><span data-stu-id="780eb-123">String</span></span>|<span data-ttu-id="780eb-124">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="780eb-124">Key of the entity.</span></span> <span data-ttu-id="780eb-125">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="780eb-125">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="780eb-126">displayName</span><span class="sxs-lookup"><span data-stu-id="780eb-126">displayName</span></span>|<span data-ttu-id="780eb-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="780eb-127">String</span></span>|<span data-ttu-id="780eb-128">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="780eb-128">The admin provided or imported title of the app.</span></span> <span data-ttu-id="780eb-129">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="780eb-129">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="780eb-130">description</span><span class="sxs-lookup"><span data-stu-id="780eb-130">description</span></span>|<span data-ttu-id="780eb-131">String</span><span class="sxs-lookup"><span data-stu-id="780eb-131">String</span></span>|<span data-ttu-id="780eb-132">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="780eb-132">The description of the app.</span></span> <span data-ttu-id="780eb-133">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="780eb-133">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="780eb-134">publicador</span><span class="sxs-lookup"><span data-stu-id="780eb-134">publisher</span></span>|<span data-ttu-id="780eb-135">String</span><span class="sxs-lookup"><span data-stu-id="780eb-135">String</span></span>|<span data-ttu-id="780eb-136">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="780eb-136">The publisher of the app.</span></span> <span data-ttu-id="780eb-137">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="780eb-137">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="780eb-138">largeIcon</span><span class="sxs-lookup"><span data-stu-id="780eb-138">largeIcon</span></span>|[<span data-ttu-id="780eb-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="780eb-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="780eb-140">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="780eb-140">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="780eb-141">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="780eb-141">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="780eb-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="780eb-142">createdDateTime</span></span>|<span data-ttu-id="780eb-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="780eb-143">DateTimeOffset</span></span>|<span data-ttu-id="780eb-144">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="780eb-144">The date and time the app was created.</span></span> <span data-ttu-id="780eb-145">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="780eb-145">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="780eb-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="780eb-146">lastModifiedDateTime</span></span>|<span data-ttu-id="780eb-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="780eb-147">DateTimeOffset</span></span>|<span data-ttu-id="780eb-148">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="780eb-148">The date and time the app was last modified.</span></span> <span data-ttu-id="780eb-149">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="780eb-149">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="780eb-150">isFeatured</span><span class="sxs-lookup"><span data-stu-id="780eb-150">isFeatured</span></span>|<span data-ttu-id="780eb-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="780eb-151">Boolean</span></span>|<span data-ttu-id="780eb-152">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="780eb-152">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="780eb-153">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="780eb-153">privacyInformationUrl</span></span>|<span data-ttu-id="780eb-154">String</span><span class="sxs-lookup"><span data-stu-id="780eb-154">String</span></span>|<span data-ttu-id="780eb-155">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="780eb-155">The privacy statement Url.</span></span> <span data-ttu-id="780eb-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="780eb-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="780eb-157">informationUrl</span><span class="sxs-lookup"><span data-stu-id="780eb-157">informationUrl</span></span>|<span data-ttu-id="780eb-158">String</span><span class="sxs-lookup"><span data-stu-id="780eb-158">String</span></span>|<span data-ttu-id="780eb-159">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="780eb-159">The more information Url.</span></span> <span data-ttu-id="780eb-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="780eb-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="780eb-161">owner</span><span class="sxs-lookup"><span data-stu-id="780eb-161">owner</span></span>|<span data-ttu-id="780eb-162">String</span><span class="sxs-lookup"><span data-stu-id="780eb-162">String</span></span>|<span data-ttu-id="780eb-163">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="780eb-163">The owner of the app.</span></span> <span data-ttu-id="780eb-164">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="780eb-164">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="780eb-165">developer</span><span class="sxs-lookup"><span data-stu-id="780eb-165">developer</span></span>|<span data-ttu-id="780eb-166">String</span><span class="sxs-lookup"><span data-stu-id="780eb-166">String</span></span>|<span data-ttu-id="780eb-167">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="780eb-167">The developer of the app.</span></span> <span data-ttu-id="780eb-168">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="780eb-168">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="780eb-169">notes</span><span class="sxs-lookup"><span data-stu-id="780eb-169">notes</span></span>|<span data-ttu-id="780eb-170">String</span><span class="sxs-lookup"><span data-stu-id="780eb-170">String</span></span>|<span data-ttu-id="780eb-171">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="780eb-171">Notes for the app.</span></span> <span data-ttu-id="780eb-172">Herdada de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="780eb-172">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="780eb-173">publishingState</span><span class="sxs-lookup"><span data-stu-id="780eb-173">publishingState</span></span>|[<span data-ttu-id="780eb-174">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="780eb-174">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="780eb-175">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="780eb-175">The publishing state for the app.</span></span> <span data-ttu-id="780eb-176">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="780eb-176">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="780eb-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="780eb-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="780eb-178">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="780eb-178">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="780eb-179">appAvailability</span><span class="sxs-lookup"><span data-stu-id="780eb-179">appAvailability</span></span>|[<span data-ttu-id="780eb-180">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="780eb-180">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="780eb-181">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="780eb-181">The Application's availability.</span></span> <span data-ttu-id="780eb-182">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="780eb-182">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="780eb-183">version</span><span class="sxs-lookup"><span data-stu-id="780eb-183">version</span></span>|<span data-ttu-id="780eb-184">String</span><span class="sxs-lookup"><span data-stu-id="780eb-184">String</span></span>|<span data-ttu-id="780eb-185">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="780eb-185">The Application's version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="780eb-186">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="780eb-186">Relationships</span></span>
|<span data-ttu-id="780eb-187">Relação</span><span class="sxs-lookup"><span data-stu-id="780eb-187">Relationship</span></span>|<span data-ttu-id="780eb-188">Tipo</span><span class="sxs-lookup"><span data-stu-id="780eb-188">Type</span></span>|<span data-ttu-id="780eb-189">Descrição</span><span class="sxs-lookup"><span data-stu-id="780eb-189">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="780eb-190">categories</span><span class="sxs-lookup"><span data-stu-id="780eb-190">categories</span></span>|<span data-ttu-id="780eb-191">Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="780eb-191">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="780eb-192">A lista de categorias para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="780eb-192">The list of categories for this app.</span></span> <span data-ttu-id="780eb-193">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="780eb-193">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="780eb-194">assignments</span><span class="sxs-lookup"><span data-stu-id="780eb-194">assignments</span></span>|<span data-ttu-id="780eb-195">Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="780eb-195">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="780eb-196">A lista de atribuições de grupo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="780eb-196">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="780eb-197">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="780eb-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="780eb-198">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="780eb-198">JSON Representation</span></span>
<span data-ttu-id="780eb-199">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="780eb-199">Here is a JSON representation of the resource.</span></span>
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




