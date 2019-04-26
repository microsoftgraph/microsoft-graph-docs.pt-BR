---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
ms.openlocfilehash: 1265432ea10e00d0456b4669d5e43e3a6ef7b1f7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343105"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="30f73-102">Tipo de recurso SharingInvitation</span><span class="sxs-lookup"><span data-stu-id="30f73-102">SharingInvitation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30f73-103">O recurso **SharingInvitation** agrupa itens de dados relacionados ao convite em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="30f73-103">The **SharingInvitation** resource groups invitation-related data items into a single strucutre.</span></span>

## <a name="json-representation"></a><span data-ttu-id="30f73-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="30f73-104">JSON representation</span></span>

<span data-ttu-id="30f73-105">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="30f73-105">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="30f73-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="30f73-106">Properties</span></span>

| <span data-ttu-id="30f73-107">Nome da Propriedade</span><span class="sxs-lookup"><span data-stu-id="30f73-107">Property Name</span></span>  | <span data-ttu-id="30f73-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="30f73-108">Type</span></span>                          | <span data-ttu-id="30f73-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="30f73-109">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="30f73-110">email</span><span class="sxs-lookup"><span data-stu-id="30f73-110">email</span></span>          | <span data-ttu-id="30f73-111">String</span><span class="sxs-lookup"><span data-stu-id="30f73-111">String</span></span>                        | <span data-ttu-id="30f73-p101">O endereço de email fornecido para o destinatário do convite de compartilhamento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="30f73-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>                                          |
| <span data-ttu-id="30f73-114">invitedBy</span><span class="sxs-lookup"><span data-stu-id="30f73-114">invitedBy</span></span>      | [<span data-ttu-id="30f73-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="30f73-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="30f73-p102">Fornece informações sobre quem enviou o convite que criou essa permissão, se essas informações estiverem disponíveis. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="30f73-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span> |
| <span data-ttu-id="30f73-118">signInRequired</span><span class="sxs-lookup"><span data-stu-id="30f73-118">signInRequired</span></span> | <span data-ttu-id="30f73-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="30f73-119">Boolean</span></span>                       | <span data-ttu-id="30f73-p103">Se `true`, o destinatário do convite precisa entrar para acessar o item compartilhado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="30f73-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>                     |

## <a name="remarks"></a><span data-ttu-id="30f73-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="30f73-122">Remarks</span></span> 

<span data-ttu-id="30f73-123">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="30f73-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


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
