---
author: JeremyKelley
description: O recurso SharingInvitation agrupa itens de dados relacionados a convites em uma única estrutura.
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 4c6a26e2acfdc4bca1eed34191ba78f333b5fc9f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997701"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="8940b-103">Tipo de recurso SharingInvitation</span><span class="sxs-lookup"><span data-stu-id="8940b-103">SharingInvitation resource type</span></span>

<span data-ttu-id="8940b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8940b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8940b-105">O recurso **SharingInvitation** agrupa itens de dados relacionados a convites em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="8940b-105">The **SharingInvitation** resource groups invitation-related data items into a single structure.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8940b-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8940b-106">JSON representation</span></span>

<span data-ttu-id="8940b-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="8940b-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sharingInvitation"
}-->

```json
{
  "email": "string",
  "invitedBy": {"@odata.type": "microsoft.graph.identitySet" },
  "signInRequired": true
}

```

## <a name="properties"></a><span data-ttu-id="8940b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8940b-108">Properties</span></span>

| <span data-ttu-id="8940b-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="8940b-109">Property Name</span></span>  | <span data-ttu-id="8940b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8940b-110">Type</span></span>                          | <span data-ttu-id="8940b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8940b-111">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8940b-112">email</span><span class="sxs-lookup"><span data-stu-id="8940b-112">email</span></span>          | <span data-ttu-id="8940b-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8940b-113">String</span></span>                        | <span data-ttu-id="8940b-p101">O endereço de email fornecido para o destinatário do convite de compartilhamento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8940b-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>                                          |
| <span data-ttu-id="8940b-116">invitedBy</span><span class="sxs-lookup"><span data-stu-id="8940b-116">invitedBy</span></span>      | [<span data-ttu-id="8940b-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="8940b-117">identitySet</span></span>](identityset.md) | <span data-ttu-id="8940b-p102">Fornece informações sobre quem enviou o convite que criou essa permissão, se essas informações estiverem disponíveis. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8940b-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span> |
| <span data-ttu-id="8940b-120">signInRequired</span><span class="sxs-lookup"><span data-stu-id="8940b-120">signInRequired</span></span> | <span data-ttu-id="8940b-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="8940b-121">Boolean</span></span>                       | <span data-ttu-id="8940b-p103">Se `true`, o destinatário do convite precisa entrar para acessar o item compartilhado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8940b-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>                     |

## <a name="remarks"></a><span data-ttu-id="8940b-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="8940b-124">Remarks</span></span> 

<span data-ttu-id="8940b-125">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="8940b-125">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


