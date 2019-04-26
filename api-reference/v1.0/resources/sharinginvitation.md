---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
ms.openlocfilehash: 0cb09136f4093b290f37ee851cb7d2d0ca10c1bf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549591"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="bf7dc-102">Tipo de recurso SharingInvitation</span><span class="sxs-lookup"><span data-stu-id="bf7dc-102">SharingInvitation resource type</span></span>

<span data-ttu-id="bf7dc-103">O recurso **SharingInvitation** agrupa itens de dados relacionados a convites em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="bf7dc-103">The **SharingInvitation** resource groups invitation-related data items into a single structure.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf7dc-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bf7dc-104">JSON representation</span></span>

<span data-ttu-id="bf7dc-105">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bf7dc-105">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="bf7dc-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bf7dc-106">Properties</span></span>

| <span data-ttu-id="bf7dc-107">Nome da Propriedade</span><span class="sxs-lookup"><span data-stu-id="bf7dc-107">Property Name</span></span>  | <span data-ttu-id="bf7dc-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf7dc-108">Type</span></span>            | <span data-ttu-id="bf7dc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf7dc-109">Description</span></span>
|:---------------|:----------------|:------------------------------------------
| <span data-ttu-id="bf7dc-110">email</span><span class="sxs-lookup"><span data-stu-id="bf7dc-110">email</span></span>          | <span data-ttu-id="bf7dc-111">String</span><span class="sxs-lookup"><span data-stu-id="bf7dc-111">String</span></span>          | <span data-ttu-id="bf7dc-p101">O endereço de email fornecido para o destinatário do convite de compartilhamento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bf7dc-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>
| <span data-ttu-id="bf7dc-114">invitedBy</span><span class="sxs-lookup"><span data-stu-id="bf7dc-114">invitedBy</span></span>      | <span data-ttu-id="bf7dc-115">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="bf7dc-115">[identitySet][]</span></span> | <span data-ttu-id="bf7dc-p102">Fornece informações sobre quem enviou o convite que criou essa permissão, se essas informações estiverem disponíveis. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bf7dc-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span>
| <span data-ttu-id="bf7dc-118">signInRequired</span><span class="sxs-lookup"><span data-stu-id="bf7dc-118">signInRequired</span></span> | <span data-ttu-id="bf7dc-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="bf7dc-119">Boolean</span></span>         | <span data-ttu-id="bf7dc-p103">Se `true`, o destinatário do convite precisa entrar para acessar o item compartilhado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bf7dc-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="bf7dc-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="bf7dc-122">Remarks</span></span>

<span data-ttu-id="bf7dc-123">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="bf7dc-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

[DriveItem]: driveitem.md
[IdentitySet]: identityset.md

<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SharingInvitation"
} -->
