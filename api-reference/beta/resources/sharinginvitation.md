---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
ms.openlocfilehash: 3ba92573aaef89b1be431ade33caa6ed465917a9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835970"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="1597a-102">Tipo de recurso SharingInvitation</span><span class="sxs-lookup"><span data-stu-id="1597a-102">SharingInvitation resource type</span></span>

> <span data-ttu-id="1597a-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1597a-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1597a-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1597a-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1597a-105">O recurso **SharingInvitation** agrupa itens de dados relacionados ao convite em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="1597a-105">The **SharingInvitation** resource groups invitation-related data items into a single strucutre.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1597a-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1597a-106">JSON representation</span></span>

<span data-ttu-id="1597a-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="1597a-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="1597a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1597a-108">Properties</span></span>

| <span data-ttu-id="1597a-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="1597a-109">Property Name</span></span>  | <span data-ttu-id="1597a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1597a-110">Type</span></span>                          | <span data-ttu-id="1597a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1597a-111">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="1597a-112">email</span><span class="sxs-lookup"><span data-stu-id="1597a-112">email</span></span>          | <span data-ttu-id="1597a-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1597a-113">String</span></span>                        | <span data-ttu-id="1597a-p102">O endereço de email fornecido para o destinatário do convite de compartilhamento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1597a-p102">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>                                          |
| <span data-ttu-id="1597a-116">invitedBy</span><span class="sxs-lookup"><span data-stu-id="1597a-116">invitedBy</span></span>      | [<span data-ttu-id="1597a-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="1597a-117">identitySet</span></span>](identityset.md) | <span data-ttu-id="1597a-p103">Fornece informações sobre quem enviou o convite que criou essa permissão, se essas informações estiverem disponíveis. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1597a-p103">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span> |
| <span data-ttu-id="1597a-120">signInRequired</span><span class="sxs-lookup"><span data-stu-id="1597a-120">signInRequired</span></span> | <span data-ttu-id="1597a-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="1597a-121">Boolean</span></span>                       | <span data-ttu-id="1597a-p104">Se `true`, o destinatário do convite precisa entrar para acessar o item compartilhado. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1597a-p104">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>                     |

## <a name="remarks"></a><span data-ttu-id="1597a-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="1597a-124">Remarks</span></span> 

<span data-ttu-id="1597a-125">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="1597a-125">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": ""
}-->
