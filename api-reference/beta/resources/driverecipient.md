---
author: JeremyKelley
description: O recurso DriveRecipient representa uma pessoa, um grupo ou outro destinatário com quem compartilhar usando a ação invite.
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f86b79567b4148934f1c9624124026472fbb3395
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012706"
---
# <a name="driverecipient-resource"></a><span data-ttu-id="8bb50-103">Recurso DriveRecipient</span><span class="sxs-lookup"><span data-stu-id="8bb50-103">DriveRecipient resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bb50-104">O recurso **DriveRecipient** representa uma pessoa, um grupo ou outro destinatário com quem compartilhar usando a ação [invite](../api/driveitem-invite.md).</span><span class="sxs-lookup"><span data-stu-id="8bb50-104">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem-invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8bb50-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8bb50-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="8bb50-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8bb50-106">Properties</span></span>
<span data-ttu-id="8bb50-107">O recurso de destinatários possui essas propriedades.</span><span class="sxs-lookup"><span data-stu-id="8bb50-107">The recipients resource has these properties.</span></span>

| <span data-ttu-id="8bb50-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="8bb50-108">Property name</span></span> | <span data-ttu-id="8bb50-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8bb50-109">Type</span></span>   | <span data-ttu-id="8bb50-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8bb50-110">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8bb50-111">email</span><span class="sxs-lookup"><span data-stu-id="8bb50-111">email</span></span>         | <span data-ttu-id="8bb50-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8bb50-112">String</span></span> | <span data-ttu-id="8bb50-113">O endereço de email do destinatário, se este tiver um endereço de email associado.</span><span class="sxs-lookup"><span data-stu-id="8bb50-113">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="8bb50-114">alias</span><span class="sxs-lookup"><span data-stu-id="8bb50-114">alias</span></span>         | <span data-ttu-id="8bb50-115">String</span><span class="sxs-lookup"><span data-stu-id="8bb50-115">String</span></span> | <span data-ttu-id="8bb50-116">O alias do objeto do domínio, para casos em que um endereço de email está indisponível (por exemplo, grupos de segurança).</span><span class="sxs-lookup"><span data-stu-id="8bb50-116">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="8bb50-117">objectId</span><span class="sxs-lookup"><span data-stu-id="8bb50-117">objectId</span></span>      | <span data-ttu-id="8bb50-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8bb50-118">String</span></span> | <span data-ttu-id="8bb50-119">O identificador exclusivo para o destinatário no diretório.</span><span class="sxs-lookup"><span data-stu-id="8bb50-119">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="8bb50-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="8bb50-120">Remarks</span></span>

<span data-ttu-id="8bb50-p101">Ao usar [invite](../api/driveitem-invite.md) para adicionar permissões, DriveRecipient pode especificar **email**, **alias** ou **objectId**. É necessário somente um desses valores.</span><span class="sxs-lookup"><span data-stu-id="8bb50-p101">When using [invite](../api/driveitem-invite.md) to add permissions, the DriveRecipient can specify **email**, **alias**, or **objectId**. Only one of these values is required.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients",
  "suppressions": []
}
-->
