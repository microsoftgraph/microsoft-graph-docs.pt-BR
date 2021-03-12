---
title: Tipo de recurso passwordCredential
description: Contém uma credencial de senha associada a um aplicativo ou uma entidade de serviço.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: f565e847cee968d07bc76399bbbcf8aeaf3d94f6
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721520"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="12388-103">Tipo de recurso passwordCredential</span><span class="sxs-lookup"><span data-stu-id="12388-103">passwordCredential resource type</span></span>

<span data-ttu-id="12388-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12388-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="12388-105">Representa uma credencial de senha associada a um aplicativo ou uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="12388-105">Represents a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="12388-106">A **propriedade passwordCredentials** do [aplicativo](application.md)</span><span class="sxs-lookup"><span data-stu-id="12388-106">The **passwordCredentials** property of the [application](application.md)</span></span> <!--and [servicePrincipal](serviceprincipal.md) entitites--> <span data-ttu-id="12388-107">entity é uma coleção de **objetos passwordCredential.**</span><span class="sxs-lookup"><span data-stu-id="12388-107">entity is a collection of **passwordCredential** objects.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="12388-108">Não há suporte para usar POST ou PATCH **para definir passwordCredential.**</span><span class="sxs-lookup"><span data-stu-id="12388-108">Using POST or PATCH to set **passwordCredential** is not supported.</span></span> <span data-ttu-id="12388-109">Use os métodos addPassword e removePassword para atualizar a senha de um aplicativo ou um servicePrincipal:</span><span class="sxs-lookup"><span data-stu-id="12388-109">Use the addPassword and removePassword methods to update the password for an application or a servicePrincipal:</span></span>
>
> - [<span data-ttu-id="12388-110">application: addPassword</span><span class="sxs-lookup"><span data-stu-id="12388-110">application: addPassword</span></span>](../api/application-addpassword.md)
> - [<span data-ttu-id="12388-111">application: removePassword</span><span class="sxs-lookup"><span data-stu-id="12388-111">application: removePassword</span></span>](../api/application-removepassword.md)
> - [<span data-ttu-id="12388-112">servicePrincipal: addPassword</span><span class="sxs-lookup"><span data-stu-id="12388-112">servicePrincipal: addPassword</span></span>](../api/serviceprincipal-addpassword.md)
> - [<span data-ttu-id="12388-113">servicePrincipal: removePassword</span><span class="sxs-lookup"><span data-stu-id="12388-113">servicePrincipal: removePassword</span></span>](../api/serviceprincipal-removepassword.md)

## <a name="properties"></a><span data-ttu-id="12388-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12388-114">Properties</span></span>
| <span data-ttu-id="12388-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12388-115">Property</span></span>     | <span data-ttu-id="12388-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="12388-116">Type</span></span>   |<span data-ttu-id="12388-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="12388-117">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="12388-118">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="12388-118">customKeyIdentifier</span></span> | <span data-ttu-id="12388-119">Binária</span><span class="sxs-lookup"><span data-stu-id="12388-119">Binary</span></span> | <span data-ttu-id="12388-120">Não usar.</span><span class="sxs-lookup"><span data-stu-id="12388-120">Do not use.</span></span> |
| <span data-ttu-id="12388-121">displayName</span><span class="sxs-lookup"><span data-stu-id="12388-121">displayName</span></span> | <span data-ttu-id="12388-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12388-122">String</span></span> | <span data-ttu-id="12388-123">Nome amigável para a senha.</span><span class="sxs-lookup"><span data-stu-id="12388-123">Friendly name for the password.</span></span> <span data-ttu-id="12388-124">Opcional.</span><span class="sxs-lookup"><span data-stu-id="12388-124">Optional.</span></span> |
| <span data-ttu-id="12388-125">endDateTime</span><span class="sxs-lookup"><span data-stu-id="12388-125">endDateTime</span></span> | <span data-ttu-id="12388-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12388-126">DateTimeOffset</span></span> | <span data-ttu-id="12388-127">A data e a hora em que a senha expira representada usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="12388-127">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="12388-128">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="12388-128">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="12388-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="12388-129">Optional.</span></span> |
| <span data-ttu-id="12388-130">dica</span><span class="sxs-lookup"><span data-stu-id="12388-130">hint</span></span> | <span data-ttu-id="12388-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12388-131">String</span></span> | <span data-ttu-id="12388-132">Contém os três primeiros caracteres da senha.</span><span class="sxs-lookup"><span data-stu-id="12388-132">Contains the first three characters of the password.</span></span> <span data-ttu-id="12388-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="12388-133">Read-only.</span></span> |
| <span data-ttu-id="12388-134">keyId</span><span class="sxs-lookup"><span data-stu-id="12388-134">keyId</span></span> | <span data-ttu-id="12388-135">Guid</span><span class="sxs-lookup"><span data-stu-id="12388-135">Guid</span></span> | <span data-ttu-id="12388-136">O identificador exclusivo da senha.</span><span class="sxs-lookup"><span data-stu-id="12388-136">The unique identifier for the password.</span></span> |
| <span data-ttu-id="12388-137">secretText</span><span class="sxs-lookup"><span data-stu-id="12388-137">secretText</span></span> | <span data-ttu-id="12388-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12388-138">String</span></span> | <span data-ttu-id="12388-139">Somente leitura; Contém as senhas fortes geradas pelo Azure AD que têm entre 16 e 64 caracteres.</span><span class="sxs-lookup"><span data-stu-id="12388-139">Read-only; Contains the strong passwords generated by Azure AD that are 16-64 characters in length.</span></span> <span data-ttu-id="12388-140">O valor de senha gerado só é retornado durante a solicitação POST inicial [para addPassword](../api/application-addpassword.md).</span><span class="sxs-lookup"><span data-stu-id="12388-140">The generated password value is only returned during the initial POST request to [addPassword](../api/application-addpassword.md).</span></span> <span data-ttu-id="12388-141">Não há como recuperar essa senha no futuro.</span><span class="sxs-lookup"><span data-stu-id="12388-141">There is no way to retrieve this password in the future.</span></span> |
| <span data-ttu-id="12388-142">startDateTime</span><span class="sxs-lookup"><span data-stu-id="12388-142">startDateTime</span></span> | <span data-ttu-id="12388-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12388-143">DateTimeOffset</span></span> | <span data-ttu-id="12388-144">A data e a hora em que a senha se torna válida.</span><span class="sxs-lookup"><span data-stu-id="12388-144">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="12388-145">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="12388-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="12388-146">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="12388-146">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="12388-147">Opcional.</span><span class="sxs-lookup"><span data-stu-id="12388-147">Optional.</span></span> |

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


## <a name="json-representation"></a><span data-ttu-id="12388-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12388-148">JSON representation</span></span>

<span data-ttu-id="12388-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="12388-149">The following is a JSON representation of the resource.</span></span>

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

