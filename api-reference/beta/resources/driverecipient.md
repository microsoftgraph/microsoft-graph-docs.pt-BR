---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ecf3e600cc943d0c82da38928d8018e6c654fb4e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525798"
---
# <a name="driverecipient-resource"></a><span data-ttu-id="0e5c8-102">Recurso DriveRecipient</span><span class="sxs-lookup"><span data-stu-id="0e5c8-102">DriveRecipient resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e5c8-103">O recurso **DriveRecipient** representa uma pessoa, um grupo ou outro destinatário com quem compartilhar usando a ação [invite](../api/driveitem-invite.md).</span><span class="sxs-lookup"><span data-stu-id="0e5c8-103">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem-invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e5c8-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0e5c8-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="0e5c8-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0e5c8-105">Properties</span></span>
<span data-ttu-id="0e5c8-106">O recurso de destinatários possui essas propriedades.</span><span class="sxs-lookup"><span data-stu-id="0e5c8-106">The recipients resource has these properties.</span></span>

| <span data-ttu-id="0e5c8-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="0e5c8-107">Property name</span></span> | <span data-ttu-id="0e5c8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e5c8-108">Type</span></span>   | <span data-ttu-id="0e5c8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e5c8-109">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0e5c8-110">email</span><span class="sxs-lookup"><span data-stu-id="0e5c8-110">email</span></span>         | <span data-ttu-id="0e5c8-111">String</span><span class="sxs-lookup"><span data-stu-id="0e5c8-111">String</span></span> | <span data-ttu-id="0e5c8-112">O endereço de email do destinatário, se este tiver um endereço de email associado.</span><span class="sxs-lookup"><span data-stu-id="0e5c8-112">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="0e5c8-113">alias</span><span class="sxs-lookup"><span data-stu-id="0e5c8-113">alias</span></span>         | <span data-ttu-id="0e5c8-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e5c8-114">String</span></span> | <span data-ttu-id="0e5c8-115">O alias do objeto do domínio, para casos em que um endereço de email está indisponível (por exemplo, grupos de segurança).</span><span class="sxs-lookup"><span data-stu-id="0e5c8-115">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="0e5c8-116">objectId</span><span class="sxs-lookup"><span data-stu-id="0e5c8-116">objectId</span></span>      | <span data-ttu-id="0e5c8-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e5c8-117">String</span></span> | <span data-ttu-id="0e5c8-118">O identificador exclusivo para o destinatário no diretório.</span><span class="sxs-lookup"><span data-stu-id="0e5c8-118">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="0e5c8-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="0e5c8-119">Remarks</span></span>

<span data-ttu-id="0e5c8-p101">Ao usar [invite](../api/driveitem-invite.md) para adicionar permissões, DriveRecipient pode especificar **email**, **alias** ou **objectId**. É necessário somente um desses valores.</span><span class="sxs-lookup"><span data-stu-id="0e5c8-p101">When using [invite](../api/driveitem-invite.md) to add permissions, the DriveRecipient can specify **email**, **alias**, or **objectId**. Only one of these values is required.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients",
  "suppressions": [
    "Error: /api-reference/beta/resources/driverecipient.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
