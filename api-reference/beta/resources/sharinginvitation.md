---
author: JeremyKelley
description: O recurso SharingInvitation agrupa itens de dados relacionados a convites em uma única estrutura.
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: eebfa17a08918ec3ac08700577921b1037761086
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008331"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="8072e-103">Tipo de recurso SharingInvitation</span><span class="sxs-lookup"><span data-stu-id="8072e-103">SharingInvitation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8072e-104">O recurso **SharingInvitation** agrupa itens de dados relacionados a convites em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="8072e-104">The **SharingInvitation** resource groups invitation-related data items into a single structure.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8072e-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8072e-105">JSON representation</span></span>

<span data-ttu-id="8072e-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="8072e-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="8072e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8072e-107">Properties</span></span>

| <span data-ttu-id="8072e-108">Nome da Propriedade</span><span class="sxs-lookup"><span data-stu-id="8072e-108">Property Name</span></span>  | <span data-ttu-id="8072e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8072e-109">Type</span></span>                          | <span data-ttu-id="8072e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8072e-110">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8072e-111">email</span><span class="sxs-lookup"><span data-stu-id="8072e-111">email</span></span>          | <span data-ttu-id="8072e-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8072e-112">String</span></span>                        | <span data-ttu-id="8072e-p101">O endereço de email fornecido para o destinatário do convite de compartilhamento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8072e-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>                                          |
| <span data-ttu-id="8072e-115">invitedBy</span><span class="sxs-lookup"><span data-stu-id="8072e-115">invitedBy</span></span>      | [<span data-ttu-id="8072e-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="8072e-116">identitySet</span></span>](identityset.md) | <span data-ttu-id="8072e-p102">Fornece informações sobre quem enviou o convite que criou essa permissão, se essas informações estiverem disponíveis. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8072e-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span> |
| <span data-ttu-id="8072e-119">signInRequired</span><span class="sxs-lookup"><span data-stu-id="8072e-119">signInRequired</span></span> | <span data-ttu-id="8072e-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="8072e-120">Boolean</span></span>                       | <span data-ttu-id="8072e-p103">Se `true`, o destinatário do convite precisa entrar para acessar o item compartilhado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8072e-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>                     |

## <a name="remarks"></a><span data-ttu-id="8072e-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="8072e-123">Remarks</span></span> 

<span data-ttu-id="8072e-124">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="8072e-124">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


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
