---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.openlocfilehash: f1bc78a8ec0648ce90221e4ad1f4473e49b625b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863725"
---
# <a name="driverecipient-resource"></a><span data-ttu-id="9e81d-102">Recurso DriveRecipient</span><span class="sxs-lookup"><span data-stu-id="9e81d-102">DriveRecipient resource</span></span>

> <span data-ttu-id="9e81d-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9e81d-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e81d-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9e81d-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9e81d-105">O recurso **DriveRecipient** representa uma pessoa, um grupo ou outro destinatário com quem compartilhar usando a ação [invite](../api/driveitem-invite.md).</span><span class="sxs-lookup"><span data-stu-id="9e81d-105">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem-invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e81d-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9e81d-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="9e81d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9e81d-107">Properties</span></span>
<span data-ttu-id="9e81d-108">O recurso de destinatários possui essas propriedades.</span><span class="sxs-lookup"><span data-stu-id="9e81d-108">The recipients resource has these properties.</span></span>

| <span data-ttu-id="9e81d-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="9e81d-109">Property name</span></span> | <span data-ttu-id="9e81d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e81d-110">Type</span></span>   | <span data-ttu-id="9e81d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e81d-111">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="9e81d-112">email</span><span class="sxs-lookup"><span data-stu-id="9e81d-112">email</span></span>         | <span data-ttu-id="9e81d-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e81d-113">String</span></span> | <span data-ttu-id="9e81d-114">O endereço de email do destinatário, se este tiver um endereço de email associado.</span><span class="sxs-lookup"><span data-stu-id="9e81d-114">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="9e81d-115">alias</span><span class="sxs-lookup"><span data-stu-id="9e81d-115">alias</span></span>         | <span data-ttu-id="9e81d-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e81d-116">String</span></span> | <span data-ttu-id="9e81d-117">O alias do objeto do domínio, para casos em que um endereço de email está indisponível (por exemplo, grupos de segurança).</span><span class="sxs-lookup"><span data-stu-id="9e81d-117">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="9e81d-118">objectId</span><span class="sxs-lookup"><span data-stu-id="9e81d-118">objectId</span></span>      | <span data-ttu-id="9e81d-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e81d-119">String</span></span> | <span data-ttu-id="9e81d-120">O identificador exclusivo para o destinatário no diretório.</span><span class="sxs-lookup"><span data-stu-id="9e81d-120">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="9e81d-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="9e81d-121">Remarks</span></span>

<span data-ttu-id="9e81d-p102">Ao usar [invite](../api/driveitem-invite.md) para adicionar permissões, DriveRecipient pode especificar **email**, **alias** ou **objectId**. É necessário somente um desses valores.</span><span class="sxs-lookup"><span data-stu-id="9e81d-p102">When using [invite](../api/driveitem-invite.md) to add permissions, the DriveRecipient can specify **email**, **alias**, or **objectId**. Only one of these values is required.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->
