---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
ms.openlocfilehash: 009dcf77492d8ec77230413dc628076ef0d557fa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523390"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="268cc-102">Tipo de recurso SharingInvitation</span><span class="sxs-lookup"><span data-stu-id="268cc-102">SharingInvitation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="268cc-103">O recurso **SharingInvitation** agrupa itens de dados relacionados ao convite em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="268cc-103">The **SharingInvitation** resource groups invitation-related data items into a single strucutre.</span></span>

## <a name="json-representation"></a><span data-ttu-id="268cc-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="268cc-104">JSON representation</span></span>

<span data-ttu-id="268cc-105">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="268cc-105">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="268cc-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="268cc-106">Properties</span></span>

| <span data-ttu-id="268cc-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="268cc-107">Property Name</span></span>  | <span data-ttu-id="268cc-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="268cc-108">Type</span></span>                          | <span data-ttu-id="268cc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="268cc-109">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="268cc-110">email</span><span class="sxs-lookup"><span data-stu-id="268cc-110">email</span></span>          | <span data-ttu-id="268cc-111">String</span><span class="sxs-lookup"><span data-stu-id="268cc-111">String</span></span>                        | <span data-ttu-id="268cc-p101">O endereço de email fornecido para o destinatário do convite de compartilhamento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="268cc-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>                                          |
| <span data-ttu-id="268cc-114">invitedBy</span><span class="sxs-lookup"><span data-stu-id="268cc-114">invitedBy</span></span>      | [<span data-ttu-id="268cc-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="268cc-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="268cc-p102">Fornece informações sobre quem enviou o convite que criou essa permissão, se essas informações estiverem disponíveis. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="268cc-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span> |
| <span data-ttu-id="268cc-118">signInRequired</span><span class="sxs-lookup"><span data-stu-id="268cc-118">signInRequired</span></span> | <span data-ttu-id="268cc-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="268cc-119">Boolean</span></span>                       | <span data-ttu-id="268cc-p103">Se `true`, o destinatário do convite precisa entrar para acessar o item compartilhado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="268cc-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>                     |

## <a name="remarks"></a><span data-ttu-id="268cc-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="268cc-122">Remarks</span></span> 

<span data-ttu-id="268cc-123">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="268cc-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharinginvitation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
