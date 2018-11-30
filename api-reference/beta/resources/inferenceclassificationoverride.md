---
title: Tipo de recurso inferenceClassificationOverride
description: Representa a substituição do usuário para como mensagens recebidas de um remetente específico sempre deve ser classificada como
ms.openlocfilehash: 63c753b7af21907717d7d9706d0606726d5670f2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034187"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="27896-103">Tipo de recurso inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="27896-103">inferenceClassificationOverride resource type</span></span>

> <span data-ttu-id="27896-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="27896-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27896-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="27896-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="27896-106">Representa a substituição de um usuário para como mensagens recebidas de um remetente específico sempre devem ser classificadas como uma [Caixa de entrada com foco](manage-focused-inbox.md).</span><span class="sxs-lookup"><span data-stu-id="27896-106">Represents a user's override for how incoming messages from a specific sender should always be classified as in a [Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="27896-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="27896-107">Methods</span></span>

| <span data-ttu-id="27896-108">Método</span><span class="sxs-lookup"><span data-stu-id="27896-108">Method</span></span>           | <span data-ttu-id="27896-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="27896-109">Return Type</span></span>    |<span data-ttu-id="27896-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="27896-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="27896-111">Update</span><span class="sxs-lookup"><span data-stu-id="27896-111">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="27896-112">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="27896-112">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="27896-113">Altere o campo **ClassifyAs** de uma substituição conforme especificado.</span><span class="sxs-lookup"><span data-stu-id="27896-113">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="27896-114">Delete</span><span class="sxs-lookup"><span data-stu-id="27896-114">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="27896-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="27896-115">None</span></span> |<span data-ttu-id="27896-116">Exclua uma substituição especificada de acordo com sua ID.</span><span class="sxs-lookup"><span data-stu-id="27896-116">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="27896-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="27896-117">Properties</span></span>
| <span data-ttu-id="27896-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27896-118">Property</span></span>     | <span data-ttu-id="27896-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="27896-119">Type</span></span>   |<span data-ttu-id="27896-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="27896-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27896-121">classifyAs</span><span class="sxs-lookup"><span data-stu-id="27896-121">classifyAs</span></span>|<span data-ttu-id="27896-122">string</span><span class="sxs-lookup"><span data-stu-id="27896-122">string</span></span>| <span data-ttu-id="27896-p102">Representa como classificar as mensagens recebidas de um remetente específico. Os valores possíveis são: `focused` e `other`.</span><span class="sxs-lookup"><span data-stu-id="27896-p102">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="27896-125">id</span><span class="sxs-lookup"><span data-stu-id="27896-125">id</span></span>|<span data-ttu-id="27896-126">string</span><span class="sxs-lookup"><span data-stu-id="27896-126">string</span></span>| <span data-ttu-id="27896-p103">O identificador exclusivo da substituição. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="27896-p103">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="27896-129">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="27896-129">senderEmailAddress</span></span>|[<span data-ttu-id="27896-130">emailAddress</span><span class="sxs-lookup"><span data-stu-id="27896-130">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="27896-131">As informações de endereço de email do remetente para quem a substituição é criada.</span><span class="sxs-lookup"><span data-stu-id="27896-131">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27896-132">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="27896-132">Relationships</span></span>
<span data-ttu-id="27896-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="27896-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="27896-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="27896-134">JSON representation</span></span>

<span data-ttu-id="27896-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="27896-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
}-->

```json
{
  "classifyAs": "string",
  "id": "string (identifier)",
  "senderEmailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->