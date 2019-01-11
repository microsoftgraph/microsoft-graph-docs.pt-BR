---
author: rgregg
ms.author: rgregg
ms.date: 09/14/2017
title: Identidade
localization_priority: Normal
ms.openlocfilehash: c1cd28f4c2932e4196605c408470948e5b570894
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847583"
---
# <a name="identity-resource-type"></a><span data-ttu-id="b12c0-102">tipo de recurso de identidade</span><span class="sxs-lookup"><span data-stu-id="b12c0-102">identity resource type</span></span>

> <span data-ttu-id="b12c0-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b12c0-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b12c0-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b12c0-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b12c0-p102">O recurso **Identity** representa uma identidade de um _actor_. Por exemplo, e ator pode ser um usuário, aplicativo ou dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b12c0-p102">The **Identity** resource represents an identity of an _actor_. For example, an actor can be a user, device, or application.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b12c0-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b12c0-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identity", "optionalProperties": ["displayName", "tenantId", "thumbnails"], "openType": true } -->

```json
{
  "displayName": "string",
  "id": "string",
  "tenantId": "string",
  "thumbnails": { "@odata.type": "microsoft.graph.thumbnailSet" }
}
```

## <a name="properties"></a><span data-ttu-id="b12c0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b12c0-108">Properties</span></span>

| <span data-ttu-id="b12c0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b12c0-109">Property</span></span>            | <span data-ttu-id="b12c0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b12c0-110">Type</span></span>   | <span data-ttu-id="b12c0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b12c0-111">Description</span></span>                                                                                                                                                                                                                                                                                                           |
|:--------------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b12c0-112">displayName</span><span class="sxs-lookup"><span data-stu-id="b12c0-112">displayName</span></span>         | <span data-ttu-id="b12c0-113">String</span><span class="sxs-lookup"><span data-stu-id="b12c0-113">String</span></span> | <span data-ttu-id="b12c0-p103">Nome de exibição da identidade. Talvez isso nem sempre esteja disponível ou atualizado. Por exemplo, se um usuário troca seu nome de exibição, a API pode mostrar o novo valor em uma resposta futura, mas os itens associados ao usuário não aparecem como tendo sido alterados ao se usar [delta](../api/driveitem-delta.md).</span><span class="sxs-lookup"><span data-stu-id="b12c0-p103">The identity's display name. Note that this may not always be available or up to date. For example, if a user changes their display name, the API may show the new value in a future response, but the items associated with the user won't show up as having changed when using [delta](../api/driveitem-delta.md).</span></span>  |
| <span data-ttu-id="b12c0-117">id</span><span class="sxs-lookup"><span data-stu-id="b12c0-117">id</span></span>                  | <span data-ttu-id="b12c0-118">String</span><span class="sxs-lookup"><span data-stu-id="b12c0-118">String</span></span> | <span data-ttu-id="b12c0-119">Identificador exclusivo da identidade.</span><span class="sxs-lookup"><span data-stu-id="b12c0-119">Unique identifier for the identity.</span></span>                                                                                                                                                                                                                                                                                   |
| <span data-ttu-id="b12c0-120">tenantId</span><span class="sxs-lookup"><span data-stu-id="b12c0-120">tenantId</span></span>            | <span data-ttu-id="b12c0-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b12c0-121">String</span></span> | <span data-ttu-id="b12c0-122">Identidade exclusiva do inquilino (opcional).</span><span class="sxs-lookup"><span data-stu-id="b12c0-122">Unique identity of the tenant (optional).</span></span>                                                                                                                                                                                                                                                                             |

## <a name="remarks"></a><span data-ttu-id="b12c0-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="b12c0-123">Remarks</span></span>

<span data-ttu-id="b12c0-p104">Em algumas circunstâncias, o identificador exclusivo para o ator pode não estar disponível. Nesse caso, a propriedade **displayName** para a identidade será retornada, mas a propriedade **id** estará ausente do recurso.</span><span class="sxs-lookup"><span data-stu-id="b12c0-p104">In some circumstances, the unique identifier for the actor may not be available. In this case, the **displayName** property for the identity will be returned, but the **id** property will be missing from the resource.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity contains information about an app, user, or group.",
  "keywords": "identity,owner,modifier,app,user,group",
  "section": "documentation",
  "tocPath": "Resources/Identity"
} -->
