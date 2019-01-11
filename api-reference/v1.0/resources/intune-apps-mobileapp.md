---
title: Tipo de recurso mobileApp
description: Uma classe abstrata que contém as propriedades base de aplicativos móveis do Intune.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: aac7045bb446956b4df415a96e5c4a7b9cbbbbae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806612"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="3482b-103">Tipo de recurso mobileApp</span><span class="sxs-lookup"><span data-stu-id="3482b-103">mobileApp resource type</span></span>

> <span data-ttu-id="3482b-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3482b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3482b-105">Uma classe abstrata que contém as propriedades base de aplicativos móveis do Intune.</span><span class="sxs-lookup"><span data-stu-id="3482b-105">An abstract class containing the base properties for Intune mobile apps.</span></span>
## <a name="methods"></a><span data-ttu-id="3482b-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="3482b-106">Methods</span></span>
|<span data-ttu-id="3482b-107">Método</span><span class="sxs-lookup"><span data-stu-id="3482b-107">Method</span></span>|<span data-ttu-id="3482b-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3482b-108">Return Type</span></span>|<span data-ttu-id="3482b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3482b-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3482b-110">Listar mobileApps</span><span class="sxs-lookup"><span data-stu-id="3482b-110">List mobileApps</span></span>](../api/intune-apps-mobileapp-list.md)|<span data-ttu-id="3482b-111">Coleção [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3482b-111">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="3482b-112">Lista propriedades e relações dos objetos [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3482b-112">List properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="3482b-113">Obter mobileApp</span><span class="sxs-lookup"><span data-stu-id="3482b-113">Get mobileApp</span></span>](../api/intune-apps-mobileapp-get.md)|[<span data-ttu-id="3482b-114">mobileApp</span><span class="sxs-lookup"><span data-stu-id="3482b-114">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="3482b-115">Propriedades de leitura e relações do objeto [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3482b-115">Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.</span></span>|
|[<span data-ttu-id="3482b-116">ação assign</span><span class="sxs-lookup"><span data-stu-id="3482b-116">assign action</span></span>](../api/intune-apps-mobileapp-assign.md)|<span data-ttu-id="3482b-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3482b-117">None</span></span>|<span data-ttu-id="3482b-118">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3482b-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="3482b-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3482b-119">Properties</span></span>
|<span data-ttu-id="3482b-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3482b-120">Property</span></span>|<span data-ttu-id="3482b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="3482b-121">Type</span></span>|<span data-ttu-id="3482b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3482b-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3482b-123">id</span><span class="sxs-lookup"><span data-stu-id="3482b-123">id</span></span>|<span data-ttu-id="3482b-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3482b-124">String</span></span>|<span data-ttu-id="3482b-125">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3482b-125">Key of the entity.</span></span>|
|<span data-ttu-id="3482b-126">displayName</span><span class="sxs-lookup"><span data-stu-id="3482b-126">displayName</span></span>|<span data-ttu-id="3482b-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3482b-127">String</span></span>|<span data-ttu-id="3482b-128">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="3482b-128">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="3482b-129">description</span><span class="sxs-lookup"><span data-stu-id="3482b-129">description</span></span>|<span data-ttu-id="3482b-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3482b-130">String</span></span>|<span data-ttu-id="3482b-131">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3482b-131">The description of the app.</span></span>|
|<span data-ttu-id="3482b-132">publisher</span><span class="sxs-lookup"><span data-stu-id="3482b-132">publisher</span></span>|<span data-ttu-id="3482b-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3482b-133">String</span></span>|<span data-ttu-id="3482b-134">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3482b-134">The publisher of the app.</span></span>|
|<span data-ttu-id="3482b-135">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3482b-135">largeIcon</span></span>|[<span data-ttu-id="3482b-136">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3482b-136">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3482b-137">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="3482b-137">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="3482b-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3482b-138">createdDateTime</span></span>|<span data-ttu-id="3482b-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3482b-139">DateTimeOffset</span></span>|<span data-ttu-id="3482b-140">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3482b-140">The date and time the app was created.</span></span>|
|<span data-ttu-id="3482b-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3482b-141">lastModifiedDateTime</span></span>|<span data-ttu-id="3482b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3482b-142">DateTimeOffset</span></span>|<span data-ttu-id="3482b-143">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3482b-143">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="3482b-144">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3482b-144">isFeatured</span></span>|<span data-ttu-id="3482b-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="3482b-145">Boolean</span></span>|<span data-ttu-id="3482b-146">O valor que indica se o aplicativo está marcado como em destaque pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="3482b-146">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="3482b-147">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3482b-147">privacyInformationUrl</span></span>|<span data-ttu-id="3482b-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3482b-148">String</span></span>|<span data-ttu-id="3482b-149">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="3482b-149">The privacy statement Url.</span></span>|
|<span data-ttu-id="3482b-150">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3482b-150">informationUrl</span></span>|<span data-ttu-id="3482b-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3482b-151">String</span></span>|<span data-ttu-id="3482b-152">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="3482b-152">The more information Url.</span></span>|
|<span data-ttu-id="3482b-153">owner</span><span class="sxs-lookup"><span data-stu-id="3482b-153">owner</span></span>|<span data-ttu-id="3482b-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3482b-154">String</span></span>|<span data-ttu-id="3482b-155">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="3482b-155">The owner of the app.</span></span>|
|<span data-ttu-id="3482b-156">developer</span><span class="sxs-lookup"><span data-stu-id="3482b-156">developer</span></span>|<span data-ttu-id="3482b-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3482b-157">String</span></span>|<span data-ttu-id="3482b-158">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3482b-158">The developer of the app.</span></span>|
|<span data-ttu-id="3482b-159">notes</span><span class="sxs-lookup"><span data-stu-id="3482b-159">notes</span></span>|<span data-ttu-id="3482b-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3482b-160">String</span></span>|<span data-ttu-id="3482b-161">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3482b-161">Notes for the app.</span></span>|
|<span data-ttu-id="3482b-162">publishingState</span><span class="sxs-lookup"><span data-stu-id="3482b-162">publishingState</span></span>|[<span data-ttu-id="3482b-163">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="3482b-163">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3482b-164">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3482b-164">The publishing state for the app.</span></span> <span data-ttu-id="3482b-165">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="3482b-165">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3482b-166">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="3482b-166">Possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3482b-167">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="3482b-167">Relationships</span></span>
|<span data-ttu-id="3482b-168">Relação</span><span class="sxs-lookup"><span data-stu-id="3482b-168">Relationship</span></span>|<span data-ttu-id="3482b-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="3482b-169">Type</span></span>|<span data-ttu-id="3482b-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="3482b-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3482b-171">categories</span><span class="sxs-lookup"><span data-stu-id="3482b-171">categories</span></span>|<span data-ttu-id="3482b-172">Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="3482b-172">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="3482b-173">A lista de categorias para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3482b-173">The list of categories for this app.</span></span>|
|<span data-ttu-id="3482b-174">assignments</span><span class="sxs-lookup"><span data-stu-id="3482b-174">assignments</span></span>|<span data-ttu-id="3482b-175">Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3482b-175">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="3482b-176">A lista de atribuições de grupo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="3482b-176">The list of group assignments for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3482b-177">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3482b-177">JSON Representation</span></span>
<span data-ttu-id="3482b-178">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3482b-178">Here is a JSON representation of the resource.</span></span>
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



