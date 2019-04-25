---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 47a080b4f81645cfe5098ec8391d58cf07fca466
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543144"
---
# <a name="driverecipient-resource"></a><span data-ttu-id="f7c0f-102">Recurso DriveRecipient</span><span class="sxs-lookup"><span data-stu-id="f7c0f-102">DriveRecipient resource</span></span>

<span data-ttu-id="f7c0f-103">O recurso **DriveRecipient** representa uma pessoa, um grupo ou outro destinatário com quem compartilhar usando a ação [invite](../api/driveitem-invite.md).</span><span class="sxs-lookup"><span data-stu-id="f7c0f-103">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem-invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7c0f-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f7c0f-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f7c0f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f7c0f-105">Properties</span></span>
<span data-ttu-id="f7c0f-106">O recurso de destinatários possui essas propriedades.</span><span class="sxs-lookup"><span data-stu-id="f7c0f-106">The recipients resource has these properties.</span></span>

| <span data-ttu-id="f7c0f-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="f7c0f-107">Property name</span></span> | <span data-ttu-id="f7c0f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7c0f-108">Type</span></span>   | <span data-ttu-id="f7c0f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7c0f-109">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f7c0f-110">email</span><span class="sxs-lookup"><span data-stu-id="f7c0f-110">email</span></span>         | <span data-ttu-id="f7c0f-111">String</span><span class="sxs-lookup"><span data-stu-id="f7c0f-111">String</span></span> | <span data-ttu-id="f7c0f-112">O endereço de email do destinatário, se este tiver um endereço de email associado.</span><span class="sxs-lookup"><span data-stu-id="f7c0f-112">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="f7c0f-113">alias</span><span class="sxs-lookup"><span data-stu-id="f7c0f-113">alias</span></span>         | <span data-ttu-id="f7c0f-114">String</span><span class="sxs-lookup"><span data-stu-id="f7c0f-114">String</span></span> | <span data-ttu-id="f7c0f-115">O alias do objeto do domínio, para casos em que um endereço de email está indisponível (por exemplo, grupos de segurança).</span><span class="sxs-lookup"><span data-stu-id="f7c0f-115">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="f7c0f-116">objectId</span><span class="sxs-lookup"><span data-stu-id="f7c0f-116">objectId</span></span>      | <span data-ttu-id="f7c0f-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7c0f-117">String</span></span> | <span data-ttu-id="f7c0f-118">O identificador exclusivo para o destinatário no diretório.</span><span class="sxs-lookup"><span data-stu-id="f7c0f-118">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="f7c0f-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="f7c0f-119">Remarks</span></span>

<span data-ttu-id="f7c0f-p101">Ao usar [invite](../api/driveitem-invite.md) para adicionar permissões, DriveRecipient pode especificar **email**, **alias** ou **objectId**. É necessário somente um desses valores.</span><span class="sxs-lookup"><span data-stu-id="f7c0f-p101">When using [invite](../api/driveitem-invite.md) to add permissions, the DriveRecipient can specify **email**, **alias**, or **objectId**. Only one of these values is required.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->
