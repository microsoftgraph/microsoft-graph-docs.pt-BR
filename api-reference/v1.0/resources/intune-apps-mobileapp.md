---
title: Tipo de recurso mobileApp
description: Uma classe abstrata que contém as propriedades base de aplicativos móveis do Intune.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1f0e2635d2b384b46a68e284daace799a196119d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531109"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="9e470-103">Tipo de recurso mobileApp</span><span class="sxs-lookup"><span data-stu-id="9e470-103">mobileApp resource type</span></span>

<span data-ttu-id="9e470-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e470-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9e470-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9e470-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e470-106">Uma classe abstrata que contém as propriedades base de aplicativos móveis do Intune.</span><span class="sxs-lookup"><span data-stu-id="9e470-106">An abstract class containing the base properties for Intune mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="9e470-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="9e470-107">Methods</span></span>
|<span data-ttu-id="9e470-108">Método</span><span class="sxs-lookup"><span data-stu-id="9e470-108">Method</span></span>|<span data-ttu-id="9e470-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9e470-109">Return Type</span></span>|<span data-ttu-id="9e470-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e470-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9e470-111">Listar mobileApps</span><span class="sxs-lookup"><span data-stu-id="9e470-111">List mobileApps</span></span>](../api/intune-apps-mobileapp-list.md)|<span data-ttu-id="9e470-112">Coleção [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9e470-112">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="9e470-113">Lista propriedades e relações dos objetos [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9e470-113">List properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="9e470-114">Obter mobileApp</span><span class="sxs-lookup"><span data-stu-id="9e470-114">Get mobileApp</span></span>](../api/intune-apps-mobileapp-get.md)|[<span data-ttu-id="9e470-115">mobileApp</span><span class="sxs-lookup"><span data-stu-id="9e470-115">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="9e470-116">Propriedades de leitura e relações do objeto [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9e470-116">Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.</span></span>|
|[<span data-ttu-id="9e470-117">ação assign</span><span class="sxs-lookup"><span data-stu-id="9e470-117">assign action</span></span>](../api/intune-apps-mobileapp-assign.md)|<span data-ttu-id="9e470-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="9e470-118">None</span></span>|<span data-ttu-id="9e470-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9e470-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="9e470-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9e470-120">Properties</span></span>
|<span data-ttu-id="9e470-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e470-121">Property</span></span>|<span data-ttu-id="9e470-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e470-122">Type</span></span>|<span data-ttu-id="9e470-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e470-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e470-124">id</span><span class="sxs-lookup"><span data-stu-id="9e470-124">id</span></span>|<span data-ttu-id="9e470-125">String</span><span class="sxs-lookup"><span data-stu-id="9e470-125">String</span></span>|<span data-ttu-id="9e470-126">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9e470-126">Key of the entity.</span></span>|
|<span data-ttu-id="9e470-127">displayName</span><span class="sxs-lookup"><span data-stu-id="9e470-127">displayName</span></span>|<span data-ttu-id="9e470-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e470-128">String</span></span>|<span data-ttu-id="9e470-129">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="9e470-129">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="9e470-130">description</span><span class="sxs-lookup"><span data-stu-id="9e470-130">description</span></span>|<span data-ttu-id="9e470-131">String</span><span class="sxs-lookup"><span data-stu-id="9e470-131">String</span></span>|<span data-ttu-id="9e470-132">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9e470-132">The description of the app.</span></span>|
|<span data-ttu-id="9e470-133">publisher</span><span class="sxs-lookup"><span data-stu-id="9e470-133">publisher</span></span>|<span data-ttu-id="9e470-134">String</span><span class="sxs-lookup"><span data-stu-id="9e470-134">String</span></span>|<span data-ttu-id="9e470-135">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9e470-135">The publisher of the app.</span></span>|
|<span data-ttu-id="9e470-136">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9e470-136">largeIcon</span></span>|[<span data-ttu-id="9e470-137">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9e470-137">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9e470-138">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="9e470-138">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="9e470-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9e470-139">createdDateTime</span></span>|<span data-ttu-id="9e470-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e470-140">DateTimeOffset</span></span>|<span data-ttu-id="9e470-141">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9e470-141">The date and time the app was created.</span></span>|
|<span data-ttu-id="9e470-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e470-142">lastModifiedDateTime</span></span>|<span data-ttu-id="9e470-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e470-143">DateTimeOffset</span></span>|<span data-ttu-id="9e470-144">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9e470-144">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="9e470-145">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9e470-145">isFeatured</span></span>|<span data-ttu-id="9e470-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="9e470-146">Boolean</span></span>|<span data-ttu-id="9e470-147">O valor que indica se o aplicativo está marcado como em destaque pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="9e470-147">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="9e470-148">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9e470-148">privacyInformationUrl</span></span>|<span data-ttu-id="9e470-149">String</span><span class="sxs-lookup"><span data-stu-id="9e470-149">String</span></span>|<span data-ttu-id="9e470-150">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="9e470-150">The privacy statement Url.</span></span>|
|<span data-ttu-id="9e470-151">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9e470-151">informationUrl</span></span>|<span data-ttu-id="9e470-152">String</span><span class="sxs-lookup"><span data-stu-id="9e470-152">String</span></span>|<span data-ttu-id="9e470-153">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="9e470-153">The more information Url.</span></span>|
|<span data-ttu-id="9e470-154">owner</span><span class="sxs-lookup"><span data-stu-id="9e470-154">owner</span></span>|<span data-ttu-id="9e470-155">String</span><span class="sxs-lookup"><span data-stu-id="9e470-155">String</span></span>|<span data-ttu-id="9e470-156">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="9e470-156">The owner of the app.</span></span>|
|<span data-ttu-id="9e470-157">developer</span><span class="sxs-lookup"><span data-stu-id="9e470-157">developer</span></span>|<span data-ttu-id="9e470-158">String</span><span class="sxs-lookup"><span data-stu-id="9e470-158">String</span></span>|<span data-ttu-id="9e470-159">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9e470-159">The developer of the app.</span></span>|
|<span data-ttu-id="9e470-160">notes</span><span class="sxs-lookup"><span data-stu-id="9e470-160">notes</span></span>|<span data-ttu-id="9e470-161">String</span><span class="sxs-lookup"><span data-stu-id="9e470-161">String</span></span>|<span data-ttu-id="9e470-162">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9e470-162">Notes for the app.</span></span>|
|<span data-ttu-id="9e470-163">publishingState</span><span class="sxs-lookup"><span data-stu-id="9e470-163">publishingState</span></span>|[<span data-ttu-id="9e470-164">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9e470-164">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9e470-165">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9e470-165">The publishing state for the app.</span></span> <span data-ttu-id="9e470-166">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="9e470-166">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9e470-167">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="9e470-167">Possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e470-168">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="9e470-168">Relationships</span></span>
|<span data-ttu-id="9e470-169">Relação</span><span class="sxs-lookup"><span data-stu-id="9e470-169">Relationship</span></span>|<span data-ttu-id="9e470-170">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e470-170">Type</span></span>|<span data-ttu-id="9e470-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e470-171">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e470-172">categories</span><span class="sxs-lookup"><span data-stu-id="9e470-172">categories</span></span>|<span data-ttu-id="9e470-173">Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="9e470-173">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="9e470-174">A lista de categorias para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9e470-174">The list of categories for this app.</span></span>|
|<span data-ttu-id="9e470-175">assignments</span><span class="sxs-lookup"><span data-stu-id="9e470-175">assignments</span></span>|<span data-ttu-id="9e470-176">Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9e470-176">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="9e470-177">A lista de atribuições de grupo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="9e470-177">The list of group assignments for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9e470-178">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9e470-178">JSON Representation</span></span>
<span data-ttu-id="9e470-179">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9e470-179">Here is a JSON representation of the resource.</span></span>
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




