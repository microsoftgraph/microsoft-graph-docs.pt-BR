---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingInvitation
ms.openlocfilehash: 75fa8212f77873b86748f6d8f63c8e62c8d6a0ca
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="dd03e-102">Tipo de recurso SharingInvitation</span><span class="sxs-lookup"><span data-stu-id="dd03e-102">SharingInvitation resource type</span></span>

<span data-ttu-id="dd03e-103">O recurso **SharingInvitation** agrupa itens de dados relacionados ao convite em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="dd03e-103">The **SharingInvitation** resource groups invitation-related data items into a single strucutre.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd03e-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dd03e-104">JSON representation</span></span>

<span data-ttu-id="dd03e-105">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="dd03e-105">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="dd03e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dd03e-106">Properties</span></span>

| <span data-ttu-id="dd03e-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="dd03e-107">Property Name</span></span>  | <span data-ttu-id="dd03e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd03e-108">Type</span></span>                          | <span data-ttu-id="dd03e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd03e-109">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="dd03e-110">email</span><span class="sxs-lookup"><span data-stu-id="dd03e-110">email</span></span>          | <span data-ttu-id="dd03e-111">String</span><span class="sxs-lookup"><span data-stu-id="dd03e-111">String</span></span>                        | <span data-ttu-id="dd03e-p101">O endereço de email fornecido para o destinatário do convite de compartilhamento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd03e-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>                                          |
| <span data-ttu-id="dd03e-114">invitedBy</span><span class="sxs-lookup"><span data-stu-id="dd03e-114">invitedBy</span></span>      | [<span data-ttu-id="dd03e-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="dd03e-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="dd03e-p102">Fornece informações sobre quem enviou o convite que criou essa permissão, se essas informações estiverem disponíveis. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd03e-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span> |
| <span data-ttu-id="dd03e-118">signInRequired</span><span class="sxs-lookup"><span data-stu-id="dd03e-118">signInRequired</span></span> | <span data-ttu-id="dd03e-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="dd03e-119">Boolean</span></span>                       | <span data-ttu-id="dd03e-p103">Se `true`, o destinatário do convite precisa entrar para acessar o item compartilhado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd03e-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>                     |

## <a name="remarks"></a><span data-ttu-id="dd03e-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="dd03e-122">Remarks</span></span> 

<span data-ttu-id="dd03e-123">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="dd03e-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SharingInvitation"
} -->
