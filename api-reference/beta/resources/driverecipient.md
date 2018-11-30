---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveRecipient
ms.openlocfilehash: c658b45ad2e99fc447459e80bfca12c29029f5b8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037570"
---
# <a name="driverecipient-resource"></a><span data-ttu-id="186c6-102">Recurso DriveRecipient</span><span class="sxs-lookup"><span data-stu-id="186c6-102">DriveRecipient resource</span></span>

> <span data-ttu-id="186c6-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="186c6-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="186c6-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="186c6-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="186c6-105">O recurso **DriveRecipient** representa uma pessoa, um grupo ou outro destinatário com quem compartilhar usando a ação [invite](../api/driveitem-invite.md).</span><span class="sxs-lookup"><span data-stu-id="186c6-105">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem-invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="186c6-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="186c6-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="186c6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="186c6-107">Properties</span></span>
<span data-ttu-id="186c6-108">O recurso de destinatários possui essas propriedades.</span><span class="sxs-lookup"><span data-stu-id="186c6-108">The recipients resource has these properties.</span></span>

| <span data-ttu-id="186c6-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="186c6-109">Property name</span></span> | <span data-ttu-id="186c6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="186c6-110">Type</span></span>   | <span data-ttu-id="186c6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="186c6-111">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="186c6-112">email</span><span class="sxs-lookup"><span data-stu-id="186c6-112">email</span></span>         | <span data-ttu-id="186c6-113">String</span><span class="sxs-lookup"><span data-stu-id="186c6-113">String</span></span> | <span data-ttu-id="186c6-114">O endereço de email do destinatário, se este tiver um endereço de email associado.</span><span class="sxs-lookup"><span data-stu-id="186c6-114">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="186c6-115">alias</span><span class="sxs-lookup"><span data-stu-id="186c6-115">alias</span></span>         | <span data-ttu-id="186c6-116">String</span><span class="sxs-lookup"><span data-stu-id="186c6-116">String</span></span> | <span data-ttu-id="186c6-117">O alias do objeto do domínio, para casos em que um endereço de email está indisponível (por exemplo, grupos de segurança).</span><span class="sxs-lookup"><span data-stu-id="186c6-117">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="186c6-118">objectId</span><span class="sxs-lookup"><span data-stu-id="186c6-118">objectId</span></span>      | <span data-ttu-id="186c6-119">String</span><span class="sxs-lookup"><span data-stu-id="186c6-119">String</span></span> | <span data-ttu-id="186c6-120">O identificador exclusivo para o destinatário no diretório.</span><span class="sxs-lookup"><span data-stu-id="186c6-120">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="186c6-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="186c6-121">Remarks</span></span>

<span data-ttu-id="186c6-p102">Ao usar [invite](../api/driveitem-invite.md) para adicionar permissões, DriveRecipient pode especificar **email**, **alias** ou **objectId**. É necessário somente um desses valores.</span><span class="sxs-lookup"><span data-stu-id="186c6-p102">When using [invite](../api/driveitem-invite.md) to add permissions, the DriveRecipient can specify **email**, **alias**, or **objectId**. Only one of these values is required.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->
