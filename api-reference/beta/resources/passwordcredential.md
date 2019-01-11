---
title: tipo de recurso passwordCredential
description: Contém uma credencial de senha associada a um aplicativo ou uma entidade de serviço. A propriedade **passwordCredentials** da entidade servicePrincipal e da entidade do aplicativo é uma coleção de **passwordCredential**.
localization_priority: Normal
ms.openlocfilehash: 5cb995c00a7dcfcfb4bda331e24dcb4d732f04f9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814438"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="c28a2-104">tipo de recurso passwordCredential</span><span class="sxs-lookup"><span data-stu-id="c28a2-104">passwordCredential resource type</span></span>

> <span data-ttu-id="c28a2-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c28a2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c28a2-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c28a2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c28a2-107">Contém uma credencial de senha associada a um aplicativo ou uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="c28a2-107">Contains a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="c28a2-108">A propriedade **passwordCredentials** da entidade [servicePrincipal](serviceprincipal.md) e da entidade do [aplicativo](application.md) é uma coleção de **passwordCredential**.</span><span class="sxs-lookup"><span data-stu-id="c28a2-108">The **passwordCredentials** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **passwordCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="c28a2-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c28a2-109">JSON representation</span></span>

<span data-ttu-id="c28a2-110">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c28a2-110">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "secretText": "string",
  "hint": "string"
}

```
## <a name="properties"></a><span data-ttu-id="c28a2-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c28a2-111">Properties</span></span>
| <span data-ttu-id="c28a2-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c28a2-112">Property</span></span>     | <span data-ttu-id="c28a2-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="c28a2-113">Type</span></span>   |<span data-ttu-id="c28a2-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="c28a2-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c28a2-115">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="c28a2-115">customKeyIdentifier</span></span>|<span data-ttu-id="c28a2-116">Binária</span><span class="sxs-lookup"><span data-stu-id="c28a2-116">Binary</span></span>|            |
|<span data-ttu-id="c28a2-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c28a2-117">endDateTime</span></span>|<span data-ttu-id="c28a2-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c28a2-118">DateTimeOffset</span></span>|<span data-ttu-id="c28a2-119">A data e hora em que a senha expira. O tipo de carimbo de hora representa as informações de data e hora usando o formato ISO 8601 e é sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="c28a2-119">The date and time at which the password expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c28a2-120">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c28a2-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c28a2-121">keyId</span><span class="sxs-lookup"><span data-stu-id="c28a2-121">keyId</span></span>|<span data-ttu-id="c28a2-122">Guid</span><span class="sxs-lookup"><span data-stu-id="c28a2-122">Guid</span></span>|            |
|<span data-ttu-id="c28a2-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c28a2-123">startDateTime</span></span>|<span data-ttu-id="c28a2-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c28a2-124">DateTimeOffset</span></span>|<span data-ttu-id="c28a2-125">A data e a hora em que a senha se torna válida. O tipo de carimbo de hora representa as informações de data e hora usando o formato ISO 8601 e é sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="c28a2-125">The date and time at which the password becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c28a2-126">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c28a2-126">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c28a2-127">secretText</span><span class="sxs-lookup"><span data-stu-id="c28a2-127">secretText</span></span>|<span data-ttu-id="c28a2-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c28a2-128">String</span></span>| <span data-ttu-id="c28a2-129">As senhas devem ser 16-64 caracteres de comprimento</span><span class="sxs-lookup"><span data-stu-id="c28a2-129">The passwords must be 16-64 characters in length</span></span> |
|<span data-ttu-id="c28a2-130">Dica</span><span class="sxs-lookup"><span data-stu-id="c28a2-130">hint</span></span>|<span data-ttu-id="c28a2-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c28a2-131">String</span></span>|  |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
