---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 4792a943598911cc2f0b8329016469ca157bda58
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480324"
---
# <a name="driverecipient-resource"></a><span data-ttu-id="ef6fb-102">Recurso DriveRecipient</span><span class="sxs-lookup"><span data-stu-id="ef6fb-102">DriveRecipient resource</span></span>

<span data-ttu-id="ef6fb-103">O recurso **DriveRecipient** representa uma pessoa, um grupo ou outro destinatário com quem compartilhar usando a ação [invite](../api/driveitem-invite.md).</span><span class="sxs-lookup"><span data-stu-id="ef6fb-103">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem-invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ef6fb-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ef6fb-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="ef6fb-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ef6fb-105">Properties</span></span>
<span data-ttu-id="ef6fb-106">O recurso de destinatários possui essas propriedades.</span><span class="sxs-lookup"><span data-stu-id="ef6fb-106">The recipients resource has these properties.</span></span>

| <span data-ttu-id="ef6fb-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="ef6fb-107">Property name</span></span> | <span data-ttu-id="ef6fb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef6fb-108">Type</span></span>   | <span data-ttu-id="ef6fb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef6fb-109">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ef6fb-110">email</span><span class="sxs-lookup"><span data-stu-id="ef6fb-110">email</span></span>         | <span data-ttu-id="ef6fb-111">String</span><span class="sxs-lookup"><span data-stu-id="ef6fb-111">String</span></span> | <span data-ttu-id="ef6fb-112">O endereço de email do destinatário, se este tiver um endereço de email associado.</span><span class="sxs-lookup"><span data-stu-id="ef6fb-112">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="ef6fb-113">alias</span><span class="sxs-lookup"><span data-stu-id="ef6fb-113">alias</span></span>         | <span data-ttu-id="ef6fb-114">String</span><span class="sxs-lookup"><span data-stu-id="ef6fb-114">String</span></span> | <span data-ttu-id="ef6fb-115">O alias do objeto do domínio, para casos em que um endereço de email está indisponível (por exemplo, grupos de segurança).</span><span class="sxs-lookup"><span data-stu-id="ef6fb-115">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="ef6fb-116">objectId</span><span class="sxs-lookup"><span data-stu-id="ef6fb-116">objectId</span></span>      | <span data-ttu-id="ef6fb-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef6fb-117">String</span></span> | <span data-ttu-id="ef6fb-118">O identificador exclusivo para o destinatário no diretório.</span><span class="sxs-lookup"><span data-stu-id="ef6fb-118">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="ef6fb-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="ef6fb-119">Remarks</span></span>

<span data-ttu-id="ef6fb-p101">Ao usar [invite](../api/driveitem-invite.md) para adicionar permissões, DriveRecipient pode especificar **email**, **alias** ou **objectId**. É necessário somente um desses valores.</span><span class="sxs-lookup"><span data-stu-id="ef6fb-p101">When using [invite](../api/driveitem-invite.md) to add permissions, the DriveRecipient can specify **email**, **alias**, or **objectId**. Only one of these values is required.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->
