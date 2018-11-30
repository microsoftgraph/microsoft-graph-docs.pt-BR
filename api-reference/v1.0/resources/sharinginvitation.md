---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingInvitation
ms.openlocfilehash: 187a7bd8fe51be57b663c215436272ee711512e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005313"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="e5dc9-102">Tipo de recurso SharingInvitation</span><span class="sxs-lookup"><span data-stu-id="e5dc9-102">SharingInvitation resource type</span></span>

<span data-ttu-id="e5dc9-103">O recurso de **SharingInvitation** agrupa itens de dados relacionados ao convite em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="e5dc9-103">The **SharingInvitation** resource groups invitation-related data items into a single structure.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5dc9-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e5dc9-104">JSON representation</span></span>

<span data-ttu-id="e5dc9-105">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e5dc9-105">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="e5dc9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e5dc9-106">Properties</span></span>

| <span data-ttu-id="e5dc9-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="e5dc9-107">Property Name</span></span>  | <span data-ttu-id="e5dc9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5dc9-108">Type</span></span>            | <span data-ttu-id="e5dc9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5dc9-109">Description</span></span>
|:---------------|:----------------|:------------------------------------------
| <span data-ttu-id="e5dc9-110">email</span><span class="sxs-lookup"><span data-stu-id="e5dc9-110">email</span></span>          | <span data-ttu-id="e5dc9-111">String</span><span class="sxs-lookup"><span data-stu-id="e5dc9-111">String</span></span>          | <span data-ttu-id="e5dc9-p101">O endereço de email fornecido para o destinatário do convite de compartilhamento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e5dc9-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>
| <span data-ttu-id="e5dc9-114">invitedBy</span><span class="sxs-lookup"><span data-stu-id="e5dc9-114">invitedBy</span></span>      | <span data-ttu-id="e5dc9-115">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="e5dc9-115">[identitySet][]</span></span> | <span data-ttu-id="e5dc9-p102">Fornece informações sobre quem enviou o convite que criou essa permissão, se essas informações estiverem disponíveis. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e5dc9-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span>
| <span data-ttu-id="e5dc9-118">signInRequired</span><span class="sxs-lookup"><span data-stu-id="e5dc9-118">signInRequired</span></span> | <span data-ttu-id="e5dc9-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="e5dc9-119">Boolean</span></span>         | <span data-ttu-id="e5dc9-p103">Se `true`, o destinatário do convite precisa entrar para acessar o item compartilhado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e5dc9-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="e5dc9-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="e5dc9-122">Remarks</span></span>

<span data-ttu-id="e5dc9-123">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="e5dc9-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

[DriveItem]: driveitem.md
[IdentitySet]: identityset.md

<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SharingInvitation"
} -->
