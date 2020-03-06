---
title: tipo de recurso passwordCredential
description: Contém uma credencial de senha associada a um aplicativo ou a uma entidade de serviço. A propriedade **passwordCredentials** da entidade servicePrincipalName e da entidade Application é uma coleção de **passwordCredential**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 0067b993cfc7d9708673bf25b20ecc054bff7925
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534076"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="598a5-104">tipo de recurso passwordCredential</span><span class="sxs-lookup"><span data-stu-id="598a5-104">passwordCredential resource type</span></span>

<span data-ttu-id="598a5-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="598a5-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="598a5-106">Representa uma credencial de senha associada a um aplicativo ou a uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="598a5-106">Represents a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="598a5-107">A propriedade **passwordCredentials** do [aplicativo](application.md)</span><span class="sxs-lookup"><span data-stu-id="598a5-107">The **passwordCredentials** property of the [application](application.md)</span></span> <!--and [servicePrincipal](serviceprincipal.md) entitites--> <span data-ttu-id="598a5-108">Entity é uma coleção de objetos **passwordCredential** .</span><span class="sxs-lookup"><span data-stu-id="598a5-108">entity is a collection of **passwordCredential** objects.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="598a5-109">Não há suporte para o uso de POST ou PATCH para definir **passwordCredential** .</span><span class="sxs-lookup"><span data-stu-id="598a5-109">Using POST or PATCH to set **passwordCredential** is not supported.</span></span> <span data-ttu-id="598a5-110">Use os métodos addpassword e removePassword para atualizar a senha de um aplicativo</span><span class="sxs-lookup"><span data-stu-id="598a5-110">Use the addPassword and removePassword methods to update the password for an application</span></span><!--or a servicePrincipal--><span data-ttu-id="598a5-111">:</span><span class="sxs-lookup"><span data-stu-id="598a5-111">:</span></span>
>
> - [<span data-ttu-id="598a5-112">Application: addpassword</span><span class="sxs-lookup"><span data-stu-id="598a5-112">application: addPassword</span></span>](../api/application-addpassword.md)
> - [<span data-ttu-id="598a5-113">aplicativo: removePassword</span><span class="sxs-lookup"><span data-stu-id="598a5-113">application: removePassword</span></span>](../api/application-removepassword.md)
<!--
> - [servicePrincipal: addPassword](../api/serviceprincipal-addpassword.md)
> - [servicePrincipal: removePassword](../api/serviceprincipal-removepassword.md)
-->

## <a name="properties"></a><span data-ttu-id="598a5-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="598a5-114">Properties</span></span>
| <span data-ttu-id="598a5-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="598a5-115">Property</span></span>     | <span data-ttu-id="598a5-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="598a5-116">Type</span></span>   |<span data-ttu-id="598a5-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="598a5-117">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="598a5-118">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="598a5-118">customKeyIdentifier</span></span> | <span data-ttu-id="598a5-119">Binária</span><span class="sxs-lookup"><span data-stu-id="598a5-119">Binary</span></span> | <span data-ttu-id="598a5-120">Não usar.</span><span class="sxs-lookup"><span data-stu-id="598a5-120">Do not use.</span></span> |
| <span data-ttu-id="598a5-121">displayName</span><span class="sxs-lookup"><span data-stu-id="598a5-121">displayName</span></span> | <span data-ttu-id="598a5-122">String</span><span class="sxs-lookup"><span data-stu-id="598a5-122">String</span></span> | <span data-ttu-id="598a5-123">Nome amigável da senha.</span><span class="sxs-lookup"><span data-stu-id="598a5-123">Friendly name for the password.</span></span> <span data-ttu-id="598a5-124">Opcional.</span><span class="sxs-lookup"><span data-stu-id="598a5-124">Optional.</span></span> |
| <span data-ttu-id="598a5-125">endDateTime</span><span class="sxs-lookup"><span data-stu-id="598a5-125">endDateTime</span></span> | <span data-ttu-id="598a5-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="598a5-126">DateTimeOffset</span></span> | <span data-ttu-id="598a5-127">A data e a hora em que a senha expira representada usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="598a5-127">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="598a5-128">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="598a5-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="598a5-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="598a5-129">Optional.</span></span> |
| <span data-ttu-id="598a5-130">Dica</span><span class="sxs-lookup"><span data-stu-id="598a5-130">hint</span></span> | <span data-ttu-id="598a5-131">String</span><span class="sxs-lookup"><span data-stu-id="598a5-131">String</span></span> | <span data-ttu-id="598a5-132">Contém os três primeiros caracteres da senha.</span><span class="sxs-lookup"><span data-stu-id="598a5-132">Contains the first three characters of the password.</span></span> <span data-ttu-id="598a5-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="598a5-133">Read-only.</span></span> |
| <span data-ttu-id="598a5-134">keyId</span><span class="sxs-lookup"><span data-stu-id="598a5-134">keyId</span></span> | <span data-ttu-id="598a5-135">Guid</span><span class="sxs-lookup"><span data-stu-id="598a5-135">Guid</span></span> | <span data-ttu-id="598a5-136">O identificador exclusivo da senha.</span><span class="sxs-lookup"><span data-stu-id="598a5-136">The unique identifier for the password.</span></span> |
| <span data-ttu-id="598a5-137">secretText</span><span class="sxs-lookup"><span data-stu-id="598a5-137">secretText</span></span> | <span data-ttu-id="598a5-138">String</span><span class="sxs-lookup"><span data-stu-id="598a5-138">String</span></span> | <span data-ttu-id="598a5-139">Somente leitura; Contém as senhas fortes geradas pelo Azure AD que têm 16-64 caracteres de comprimento.</span><span class="sxs-lookup"><span data-stu-id="598a5-139">Read-only; Contains the strong passwords generated by Azure AD that are 16-64 characters in length.</span></span> <span data-ttu-id="598a5-140">O valor da senha gerada só é retornado durante a solicitação POST inicial para [addpassword](../api/application-addpassword.md).</span><span class="sxs-lookup"><span data-stu-id="598a5-140">The generated password value is only returned during the initial POST request to [addPassword](../api/application-addpassword.md).</span></span> <span data-ttu-id="598a5-141">Não há como recuperar essa senha no futuro.</span><span class="sxs-lookup"><span data-stu-id="598a5-141">There is no way to retrieve this password in the future.</span></span> |
| <span data-ttu-id="598a5-142">startDateTime</span><span class="sxs-lookup"><span data-stu-id="598a5-142">startDateTime</span></span> | <span data-ttu-id="598a5-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="598a5-143">DateTimeOffset</span></span> | <span data-ttu-id="598a5-144">A data e a hora em que a senha se torna válida.</span><span class="sxs-lookup"><span data-stu-id="598a5-144">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="598a5-145">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="598a5-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="598a5-146">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="598a5-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="598a5-147">Opcional.</span><span class="sxs-lookup"><span data-stu-id="598a5-147">Optional.</span></span> |

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


## <a name="json-representation"></a><span data-ttu-id="598a5-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="598a5-148">JSON representation</span></span>

<span data-ttu-id="598a5-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="598a5-149">The following is a JSON representation of the resource.</span></span>

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
