---
title: tipo de recurso passwordCredential
description: Contém uma credencial de senha associada a um aplicativo ou a uma entidade de serviço.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 25b2070a7a665bf6893ad870a7a3111ae9eba80f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998212"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="a9e65-103">tipo de recurso passwordCredential</span><span class="sxs-lookup"><span data-stu-id="a9e65-103">passwordCredential resource type</span></span>

<span data-ttu-id="a9e65-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9e65-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9e65-105">Representa uma credencial de senha associada a um aplicativo ou a uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="a9e65-105">Represents a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="a9e65-106">A propriedade **passwordCredentials** do [aplicativo](application.md) e do entitites do [servicePrincipalName](serviceprincipal.md) é uma coleção de objetos **passwordCredential** .</span><span class="sxs-lookup"><span data-stu-id="a9e65-106">The **passwordCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entitites is a collection of **passwordCredential** objects.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a9e65-107">Não há suporte para o uso de POST ou PATCH para definir **passwordCredential** .</span><span class="sxs-lookup"><span data-stu-id="a9e65-107">Using POST or PATCH to set **passwordCredential** is not supported.</span></span> <span data-ttu-id="a9e65-108">Use os métodos addpassword e removePassword para atualizar a senha de um aplicativo ou de um servicePrincipalName:</span><span class="sxs-lookup"><span data-stu-id="a9e65-108">Use the addPassword and removePassword methods to update the password for an application or a servicePrincipal:</span></span>
>
> - [<span data-ttu-id="a9e65-109">Application: addpassword</span><span class="sxs-lookup"><span data-stu-id="a9e65-109">application: addPassword</span></span>](../api/application-addpassword.md)
> - [<span data-ttu-id="a9e65-110">aplicativo: removePassword</span><span class="sxs-lookup"><span data-stu-id="a9e65-110">application: removePassword</span></span>](../api/application-removepassword.md)
> - [<span data-ttu-id="a9e65-111">servicePrincipalName: addpassword</span><span class="sxs-lookup"><span data-stu-id="a9e65-111">servicePrincipal: addPassword</span></span>](../api/serviceprincipal-addpassword.md)
> - [<span data-ttu-id="a9e65-112">servicePrincipalName: removePassword</span><span class="sxs-lookup"><span data-stu-id="a9e65-112">servicePrincipal: removePassword</span></span>](../api/serviceprincipal-removepassword.md)


## <a name="properties"></a><span data-ttu-id="a9e65-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a9e65-113">Properties</span></span>
| <span data-ttu-id="a9e65-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9e65-114">Property</span></span>     | <span data-ttu-id="a9e65-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9e65-115">Type</span></span>   |<span data-ttu-id="a9e65-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9e65-116">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a9e65-117">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="a9e65-117">customKeyIdentifier</span></span> | <span data-ttu-id="a9e65-118">Binária</span><span class="sxs-lookup"><span data-stu-id="a9e65-118">Binary</span></span> | <span data-ttu-id="a9e65-119">Não usar.</span><span class="sxs-lookup"><span data-stu-id="a9e65-119">Do not use.</span></span> |
| <span data-ttu-id="a9e65-120">displayName</span><span class="sxs-lookup"><span data-stu-id="a9e65-120">displayName</span></span> | <span data-ttu-id="a9e65-121">String</span><span class="sxs-lookup"><span data-stu-id="a9e65-121">String</span></span> | <span data-ttu-id="a9e65-122">Nome amigável da senha.</span><span class="sxs-lookup"><span data-stu-id="a9e65-122">Friendly name for the password.</span></span> <span data-ttu-id="a9e65-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a9e65-123">Optional.</span></span> |
| <span data-ttu-id="a9e65-124">endDateTime</span><span class="sxs-lookup"><span data-stu-id="a9e65-124">endDateTime</span></span> | <span data-ttu-id="a9e65-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9e65-125">DateTimeOffset</span></span> | <span data-ttu-id="a9e65-126">A data e a hora em que a senha expira representada usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="a9e65-126">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a9e65-127">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a9e65-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="a9e65-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a9e65-128">Optional.</span></span> |
| <span data-ttu-id="a9e65-129">Dica</span><span class="sxs-lookup"><span data-stu-id="a9e65-129">hint</span></span> | <span data-ttu-id="a9e65-130">String</span><span class="sxs-lookup"><span data-stu-id="a9e65-130">String</span></span> | <span data-ttu-id="a9e65-131">Contém os três primeiros caracteres da senha.</span><span class="sxs-lookup"><span data-stu-id="a9e65-131">Contains the first three characters of the password.</span></span> <span data-ttu-id="a9e65-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a9e65-132">Read-only.</span></span> |
| <span data-ttu-id="a9e65-133">keyId</span><span class="sxs-lookup"><span data-stu-id="a9e65-133">keyId</span></span> | <span data-ttu-id="a9e65-134">Guid</span><span class="sxs-lookup"><span data-stu-id="a9e65-134">Guid</span></span> | <span data-ttu-id="a9e65-135">O identificador exclusivo da senha.</span><span class="sxs-lookup"><span data-stu-id="a9e65-135">The unique identifier for the password.</span></span> |
| <span data-ttu-id="a9e65-136">secretText</span><span class="sxs-lookup"><span data-stu-id="a9e65-136">secretText</span></span> | <span data-ttu-id="a9e65-137">String</span><span class="sxs-lookup"><span data-stu-id="a9e65-137">String</span></span> | <span data-ttu-id="a9e65-138">Somente leitura; Contém as senhas fortes geradas pelo Azure AD que têm 16-64 caracteres de comprimento.</span><span class="sxs-lookup"><span data-stu-id="a9e65-138">Read-only; Contains the strong passwords generated by Azure AD that are 16-64 characters in length.</span></span> <span data-ttu-id="a9e65-139">O valor da senha gerada só é retornado durante a solicitação POST inicial para [addpassword](../api/application-addpassword.md).</span><span class="sxs-lookup"><span data-stu-id="a9e65-139">The generated password value is only returned during the initial POST request to [addPassword](../api/application-addpassword.md).</span></span> <span data-ttu-id="a9e65-140">Não há como recuperar essa senha no futuro.</span><span class="sxs-lookup"><span data-stu-id="a9e65-140">There is no way to retrieve this password in the future.</span></span> |
| <span data-ttu-id="a9e65-141">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a9e65-141">startDateTime</span></span> | <span data-ttu-id="a9e65-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9e65-142">DateTimeOffset</span></span> | <span data-ttu-id="a9e65-143">A data e a hora em que a senha se torna válida.</span><span class="sxs-lookup"><span data-stu-id="a9e65-143">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="a9e65-144">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="a9e65-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a9e65-145">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a9e65-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="a9e65-146">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a9e65-146">Optional.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


## <a name="json-representation"></a><span data-ttu-id="a9e65-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a9e65-147">JSON representation</span></span>

<span data-ttu-id="a9e65-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a9e65-148">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordCredential",
  "baseType": null
}-->

```json
{
  "customKeyIdentifier": "Binary",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "hint": "String",
  "keyId": "Guid",
  "secretText": "String",
  "startDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


