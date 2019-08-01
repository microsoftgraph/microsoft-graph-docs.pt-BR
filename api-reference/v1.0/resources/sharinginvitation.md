---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
description: O recurso SharingInvitation agrupa itens de dados relacionados a convites em uma única estrutura.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 011402b40b601642a048b91e3b3f66de0792aaf2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034241"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="c1394-103">Tipo de recurso SharingInvitation</span><span class="sxs-lookup"><span data-stu-id="c1394-103">SharingInvitation resource type</span></span>

<span data-ttu-id="c1394-104">O recurso **SharingInvitation** agrupa itens de dados relacionados a convites em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="c1394-104">The **SharingInvitation** resource groups invitation-related data items into a single structure.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1394-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c1394-105">JSON representation</span></span>

<span data-ttu-id="c1394-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c1394-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="c1394-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c1394-107">Properties</span></span>

| <span data-ttu-id="c1394-108">Nome da Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1394-108">Property Name</span></span>  | <span data-ttu-id="c1394-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1394-109">Type</span></span>            | <span data-ttu-id="c1394-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1394-110">Description</span></span>
|:---------------|:----------------|:------------------------------------------
| <span data-ttu-id="c1394-111">email</span><span class="sxs-lookup"><span data-stu-id="c1394-111">email</span></span>          | <span data-ttu-id="c1394-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1394-112">String</span></span>          | <span data-ttu-id="c1394-p101">O endereço de email fornecido para o destinatário do convite de compartilhamento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c1394-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>
| <span data-ttu-id="c1394-115">invitedBy</span><span class="sxs-lookup"><span data-stu-id="c1394-115">invitedBy</span></span>      | <span data-ttu-id="c1394-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="c1394-116">[identitySet][]</span></span> | <span data-ttu-id="c1394-p102">Fornece informações sobre quem enviou o convite que criou essa permissão, se essas informações estiverem disponíveis. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c1394-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span>
| <span data-ttu-id="c1394-119">signInRequired</span><span class="sxs-lookup"><span data-stu-id="c1394-119">signInRequired</span></span> | <span data-ttu-id="c1394-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="c1394-120">Boolean</span></span>         | <span data-ttu-id="c1394-p103">Se `true`, o destinatário do convite precisa entrar para acessar o item compartilhado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c1394-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="c1394-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="c1394-123">Remarks</span></span>

<span data-ttu-id="c1394-124">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="c1394-124">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

[DriveItem]: driveitem.md
[IdentitySet]: identityset.md

<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SharingInvitation"
} -->
