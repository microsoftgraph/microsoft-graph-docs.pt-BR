---
title: Tipo de recurso mobileApp
description: Uma classe abstrata que contém as propriedades base de aplicativos móveis do Intune.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 08bc3cb0c6b1a7b815e30179aa79861b08ad3b15
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028949"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="e2f97-103">Tipo de recurso mobileApp</span><span class="sxs-lookup"><span data-stu-id="e2f97-103">mobileApp resource type</span></span>

> <span data-ttu-id="e2f97-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e2f97-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2f97-105">Uma classe abstrata que contém as propriedades base de aplicativos móveis do Intune.</span><span class="sxs-lookup"><span data-stu-id="e2f97-105">An abstract class containing the base properties for Intune mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="e2f97-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="e2f97-106">Methods</span></span>
|<span data-ttu-id="e2f97-107">Método</span><span class="sxs-lookup"><span data-stu-id="e2f97-107">Method</span></span>|<span data-ttu-id="e2f97-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e2f97-108">Return Type</span></span>|<span data-ttu-id="e2f97-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2f97-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e2f97-110">Listar mobileApps</span><span class="sxs-lookup"><span data-stu-id="e2f97-110">List mobileApps</span></span>](../api/intune-apps-mobileapp-list.md)|<span data-ttu-id="e2f97-111">Coleção [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2f97-111">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="e2f97-112">Lista propriedades e relações dos objetos [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e2f97-112">List properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="e2f97-113">Obter mobileApp</span><span class="sxs-lookup"><span data-stu-id="e2f97-113">Get mobileApp</span></span>](../api/intune-apps-mobileapp-get.md)|[<span data-ttu-id="e2f97-114">mobileApp</span><span class="sxs-lookup"><span data-stu-id="e2f97-114">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="e2f97-115">Propriedades de leitura e relações do objeto [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e2f97-115">Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.</span></span>|
|[<span data-ttu-id="e2f97-116">ação assign</span><span class="sxs-lookup"><span data-stu-id="e2f97-116">assign action</span></span>](../api/intune-apps-mobileapp-assign.md)|<span data-ttu-id="e2f97-117">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e2f97-117">None</span></span>|<span data-ttu-id="e2f97-118">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e2f97-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e2f97-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2f97-119">Properties</span></span>
|<span data-ttu-id="e2f97-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2f97-120">Property</span></span>|<span data-ttu-id="e2f97-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2f97-121">Type</span></span>|<span data-ttu-id="e2f97-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2f97-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2f97-123">id</span><span class="sxs-lookup"><span data-stu-id="e2f97-123">id</span></span>|<span data-ttu-id="e2f97-124">String</span><span class="sxs-lookup"><span data-stu-id="e2f97-124">String</span></span>|<span data-ttu-id="e2f97-125">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e2f97-125">Key of the entity.</span></span>|
|<span data-ttu-id="e2f97-126">displayName</span><span class="sxs-lookup"><span data-stu-id="e2f97-126">displayName</span></span>|<span data-ttu-id="e2f97-127">String</span><span class="sxs-lookup"><span data-stu-id="e2f97-127">String</span></span>|<span data-ttu-id="e2f97-128">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="e2f97-128">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="e2f97-129">descrição</span><span class="sxs-lookup"><span data-stu-id="e2f97-129">description</span></span>|<span data-ttu-id="e2f97-130">String</span><span class="sxs-lookup"><span data-stu-id="e2f97-130">String</span></span>|<span data-ttu-id="e2f97-131">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e2f97-131">The description of the app.</span></span>|
|<span data-ttu-id="e2f97-132">publisher</span><span class="sxs-lookup"><span data-stu-id="e2f97-132">publisher</span></span>|<span data-ttu-id="e2f97-133">String</span><span class="sxs-lookup"><span data-stu-id="e2f97-133">String</span></span>|<span data-ttu-id="e2f97-134">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e2f97-134">The publisher of the app.</span></span>|
|<span data-ttu-id="e2f97-135">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e2f97-135">largeIcon</span></span>|[<span data-ttu-id="e2f97-136">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e2f97-136">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e2f97-137">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="e2f97-137">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="e2f97-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2f97-138">createdDateTime</span></span>|<span data-ttu-id="e2f97-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2f97-139">DateTimeOffset</span></span>|<span data-ttu-id="e2f97-140">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e2f97-140">The date and time the app was created.</span></span>|
|<span data-ttu-id="e2f97-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2f97-141">lastModifiedDateTime</span></span>|<span data-ttu-id="e2f97-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2f97-142">DateTimeOffset</span></span>|<span data-ttu-id="e2f97-143">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e2f97-143">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="e2f97-144">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e2f97-144">isFeatured</span></span>|<span data-ttu-id="e2f97-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2f97-145">Boolean</span></span>|<span data-ttu-id="e2f97-146">O valor que indica se o aplicativo está marcado como em destaque pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="e2f97-146">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="e2f97-147">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e2f97-147">privacyInformationUrl</span></span>|<span data-ttu-id="e2f97-148">String</span><span class="sxs-lookup"><span data-stu-id="e2f97-148">String</span></span>|<span data-ttu-id="e2f97-149">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="e2f97-149">The privacy statement Url.</span></span>|
|<span data-ttu-id="e2f97-150">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e2f97-150">informationUrl</span></span>|<span data-ttu-id="e2f97-151">String</span><span class="sxs-lookup"><span data-stu-id="e2f97-151">String</span></span>|<span data-ttu-id="e2f97-152">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="e2f97-152">The more information Url.</span></span>|
|<span data-ttu-id="e2f97-153">owner</span><span class="sxs-lookup"><span data-stu-id="e2f97-153">owner</span></span>|<span data-ttu-id="e2f97-154">String</span><span class="sxs-lookup"><span data-stu-id="e2f97-154">String</span></span>|<span data-ttu-id="e2f97-155">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e2f97-155">The owner of the app.</span></span>|
|<span data-ttu-id="e2f97-156">developer</span><span class="sxs-lookup"><span data-stu-id="e2f97-156">developer</span></span>|<span data-ttu-id="e2f97-157">String</span><span class="sxs-lookup"><span data-stu-id="e2f97-157">String</span></span>|<span data-ttu-id="e2f97-158">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e2f97-158">The developer of the app.</span></span>|
|<span data-ttu-id="e2f97-159">notes</span><span class="sxs-lookup"><span data-stu-id="e2f97-159">notes</span></span>|<span data-ttu-id="e2f97-160">String</span><span class="sxs-lookup"><span data-stu-id="e2f97-160">String</span></span>|<span data-ttu-id="e2f97-161">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e2f97-161">Notes for the app.</span></span>|
|<span data-ttu-id="e2f97-162">publishingState</span><span class="sxs-lookup"><span data-stu-id="e2f97-162">publishingState</span></span>|[<span data-ttu-id="e2f97-163">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e2f97-163">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e2f97-164">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e2f97-164">The publishing state for the app.</span></span> <span data-ttu-id="e2f97-165">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="e2f97-165">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e2f97-166">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e2f97-166">Possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2f97-167">Relações</span><span class="sxs-lookup"><span data-stu-id="e2f97-167">Relationships</span></span>
|<span data-ttu-id="e2f97-168">Relação</span><span class="sxs-lookup"><span data-stu-id="e2f97-168">Relationship</span></span>|<span data-ttu-id="e2f97-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2f97-169">Type</span></span>|<span data-ttu-id="e2f97-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2f97-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2f97-171">categories</span><span class="sxs-lookup"><span data-stu-id="e2f97-171">categories</span></span>|<span data-ttu-id="e2f97-172">Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="e2f97-172">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="e2f97-173">A lista de categorias para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e2f97-173">The list of categories for this app.</span></span>|
|<span data-ttu-id="e2f97-174">assignments</span><span class="sxs-lookup"><span data-stu-id="e2f97-174">assignments</span></span>|<span data-ttu-id="e2f97-175">Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e2f97-175">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="e2f97-176">A lista de atribuições de grupo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="e2f97-176">The list of group assignments for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2f97-177">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2f97-177">JSON Representation</span></span>
<span data-ttu-id="e2f97-178">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e2f97-178">Here is a JSON representation of the resource.</span></span>
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
  "publishingState": "String"
}
```



