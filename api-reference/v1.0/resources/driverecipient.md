---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
description: O recurso DriveRecipient representa uma pessoa, um grupo ou outro destinatário com quem compartilhar usando a ação invite.
doc_type: resourcePageType
ms.openlocfilehash: d1b123c897791dff5bd6c42eb9e4b030e83e1d5c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531528"
---
# <a name="driverecipient-resource"></a><span data-ttu-id="ba2e5-103">Recurso DriveRecipient</span><span class="sxs-lookup"><span data-stu-id="ba2e5-103">DriveRecipient resource</span></span>

<span data-ttu-id="ba2e5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba2e5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ba2e5-105">O recurso **DriveRecipient** representa uma pessoa, um grupo ou outro destinatário com quem compartilhar usando a ação [invite](../api/driveitem-invite.md).</span><span class="sxs-lookup"><span data-stu-id="ba2e5-105">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem-invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba2e5-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ba2e5-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="ba2e5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ba2e5-107">Properties</span></span>
<span data-ttu-id="ba2e5-108">O recurso de destinatários possui essas propriedades.</span><span class="sxs-lookup"><span data-stu-id="ba2e5-108">The recipients resource has these properties.</span></span>

| <span data-ttu-id="ba2e5-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="ba2e5-109">Property name</span></span> | <span data-ttu-id="ba2e5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba2e5-110">Type</span></span>   | <span data-ttu-id="ba2e5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba2e5-111">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ba2e5-112">email</span><span class="sxs-lookup"><span data-stu-id="ba2e5-112">email</span></span>         | <span data-ttu-id="ba2e5-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba2e5-113">String</span></span> | <span data-ttu-id="ba2e5-114">O endereço de email do destinatário, se este tiver um endereço de email associado.</span><span class="sxs-lookup"><span data-stu-id="ba2e5-114">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="ba2e5-115">alias</span><span class="sxs-lookup"><span data-stu-id="ba2e5-115">alias</span></span>         | <span data-ttu-id="ba2e5-116">String</span><span class="sxs-lookup"><span data-stu-id="ba2e5-116">String</span></span> | <span data-ttu-id="ba2e5-117">O alias do objeto do domínio, para casos em que um endereço de email está indisponível (por exemplo, grupos de segurança).</span><span class="sxs-lookup"><span data-stu-id="ba2e5-117">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="ba2e5-118">objectId</span><span class="sxs-lookup"><span data-stu-id="ba2e5-118">objectId</span></span>      | <span data-ttu-id="ba2e5-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba2e5-119">String</span></span> | <span data-ttu-id="ba2e5-120">O identificador exclusivo para o destinatário no diretório.</span><span class="sxs-lookup"><span data-stu-id="ba2e5-120">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="ba2e5-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="ba2e5-121">Remarks</span></span>

<span data-ttu-id="ba2e5-p101">Ao usar [invite](../api/driveitem-invite.md) para adicionar permissões, DriveRecipient pode especificar **email**, **alias** ou **objectId**. É necessário somente um desses valores.</span><span class="sxs-lookup"><span data-stu-id="ba2e5-p101">When using [invite](../api/driveitem-invite.md) to add permissions, the DriveRecipient can specify **email**, **alias**, or **objectId**. Only one of these values is required.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->
