---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveRecipient
ms.openlocfilehash: 53f6a5559cb90142a88b839a996cb2eedfd1037a
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="driverecipient-resource"></a><span data-ttu-id="0af9d-102">Recurso DriveRecipient</span><span class="sxs-lookup"><span data-stu-id="0af9d-102">DriveRecipient resource type</span></span>

<span data-ttu-id="0af9d-103">O recurso **DriveRecipient** representa uma pessoa, um grupo ou outro destinatário com quem compartilhar usando a ação [invite](../api/driveitem_invite.md).</span><span class="sxs-lookup"><span data-stu-id="0af9d-103">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem_invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0af9d-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0af9d-104">JSON representation</span></span>

<!-- { 
  "blockType": "resource", 
  "@odata.type": "microsoft.graph.driveRecipient", 
  "optionalProperties": ["alias", "objectId", "email"] } -->
```json
{
  "email": "string",
  "alias": "string",
  "objectId": "string",
}
```

## <a name="properties"></a><span data-ttu-id="0af9d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0af9d-105">Properties</span></span>
<span data-ttu-id="0af9d-106">O recurso de destinatários possui essas propriedades.</span><span class="sxs-lookup"><span data-stu-id="0af9d-106">The recipients resource has these properties.</span></span>

| <span data-ttu-id="0af9d-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="0af9d-107">Property name</span></span> | <span data-ttu-id="0af9d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0af9d-108">Type</span></span>   | <span data-ttu-id="0af9d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0af9d-109">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0af9d-110">email</span><span class="sxs-lookup"><span data-stu-id="0af9d-110">email</span></span>         | <span data-ttu-id="0af9d-111">String</span><span class="sxs-lookup"><span data-stu-id="0af9d-111">String</span></span> | <span data-ttu-id="0af9d-112">O endereço de email do destinatário, se este tiver um endereço de email associado.</span><span class="sxs-lookup"><span data-stu-id="0af9d-112">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="0af9d-113">alias</span><span class="sxs-lookup"><span data-stu-id="0af9d-113">alias</span></span>         | <span data-ttu-id="0af9d-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0af9d-114">String</span></span> | <span data-ttu-id="0af9d-115">O alias do objeto do domínio, para casos em que um endereço de email está indisponível (por exemplo, grupos de segurança).</span><span class="sxs-lookup"><span data-stu-id="0af9d-115">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="0af9d-116">objectId</span><span class="sxs-lookup"><span data-stu-id="0af9d-116">objectId</span></span>      | <span data-ttu-id="0af9d-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0af9d-117">String</span></span> | <span data-ttu-id="0af9d-118">O identificador exclusivo para o destinatário no diretório.</span><span class="sxs-lookup"><span data-stu-id="0af9d-118">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="0af9d-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="0af9d-119">Remarks</span></span>

<span data-ttu-id="0af9d-120">Ao usar [invite](../api/driveitem_invite.md) para adicionar permissões, DriveRecipient pode especificar **email**, **alias** ou **objectId**.</span><span class="sxs-lookup"><span data-stu-id="0af9d-120">When using invite to add permissions, the DriveRecipient can specify email, alias, or objectId. Only one of these values is required.</span></span>
<span data-ttu-id="0af9d-121">É necessário somente um desses valores.</span><span class="sxs-lookup"><span data-stu-id="0af9d-121">Only one of these values is required.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->
