---
title: tipo de recurso contratofile
description: Representa um arquivo de contrato de uso personalizável que um locatário gerencia com o Azure Active Directory (Azure AD). Ele contém metadados sobre o arquivo de contrato (por exemplo, o nome, o idioma e se é o arquivo padrão).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: 12c45876558a162b910120e62c6997c251f391e1
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49664020"
---
# <a name="agreementfile-resource-type"></a><span data-ttu-id="2056d-104">tipo de recurso contratofile</span><span class="sxs-lookup"><span data-stu-id="2056d-104">agreementFile resource type</span></span>

<span data-ttu-id="2056d-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2056d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2056d-106">Representa um arquivo de contrato de uso personalizável que um locatário gerencia com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="2056d-106">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="2056d-107">Ele contém metadados sobre o arquivo de contrato (por exemplo, o nome, o idioma e se é o arquivo padrão).</span><span class="sxs-lookup"><span data-stu-id="2056d-107">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a><span data-ttu-id="2056d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2056d-108">Properties</span></span>
| <span data-ttu-id="2056d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2056d-109">Property</span></span>     | <span data-ttu-id="2056d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2056d-110">Type</span></span>        | <span data-ttu-id="2056d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2056d-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2056d-112">fileData</span><span class="sxs-lookup"><span data-stu-id="2056d-112">fileData</span></span>|[<span data-ttu-id="2056d-113">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="2056d-113">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="2056d-114">Dados que representam o documento PDF termos de uso.</span><span class="sxs-lookup"><span data-stu-id="2056d-114">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="2056d-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2056d-115">Read-only.</span></span>|
|<span data-ttu-id="2056d-116">fileName</span><span class="sxs-lookup"><span data-stu-id="2056d-116">fileName</span></span>|<span data-ttu-id="2056d-117">String</span><span class="sxs-lookup"><span data-stu-id="2056d-117">String</span></span>|<span data-ttu-id="2056d-118">Nome do arquivo de contrato (por exemplo, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="2056d-118">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="2056d-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2056d-119">Read-only.</span></span>|
|<span data-ttu-id="2056d-120">id</span><span class="sxs-lookup"><span data-stu-id="2056d-120">id</span></span>|<span data-ttu-id="2056d-121">String</span><span class="sxs-lookup"><span data-stu-id="2056d-121">String</span></span>|<span data-ttu-id="2056d-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2056d-122">Read-only.</span></span>|
|<span data-ttu-id="2056d-123">isDefault</span><span class="sxs-lookup"><span data-stu-id="2056d-123">isDefault</span></span>|<span data-ttu-id="2056d-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="2056d-124">Boolean</span></span>|<span data-ttu-id="2056d-125">Indica se este é o arquivo de contrato padrão se nenhuma das culturas corresponder à preferência do cliente.</span><span class="sxs-lookup"><span data-stu-id="2056d-125">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="2056d-126">Se nenhum dos arquivos estiver marcado como padrão, o primeiro será tratado como o padrão.</span><span class="sxs-lookup"><span data-stu-id="2056d-126">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="2056d-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2056d-127">Read-only.</span></span>|
|<span data-ttu-id="2056d-128">idioma</span><span class="sxs-lookup"><span data-stu-id="2056d-128">language</span></span>|<span data-ttu-id="2056d-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2056d-129">String</span></span>|<span data-ttu-id="2056d-130">Cultura do arquivo de contrato no formato languagecode2-Country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="2056d-130">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="2056d-131">languagecode2 é um código de duas letras em minúsculas derivado de ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="2056d-131">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="2056d-132">Country/regioncode2 é derivado de ISO 3166 e geralmente consiste em duas letras maiúsculas ou uma marca de idioma BCP-47 (por exemplo, en-US).</span><span class="sxs-lookup"><span data-stu-id="2056d-132">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="2056d-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2056d-133">Read-only.</span></span>|
|<span data-ttu-id="2056d-134">isMajorVersion</span><span class="sxs-lookup"><span data-stu-id="2056d-134">isMajorVersion</span></span>|<span data-ttu-id="2056d-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="2056d-135">Boolean</span></span>|<span data-ttu-id="2056d-136">Indica se o arquivo de contrato é uma atualização de versão principal.</span><span class="sxs-lookup"><span data-stu-id="2056d-136">Indicates whether the agreement file is a major version update.</span></span> <span data-ttu-id="2056d-137">As atualizações de versão principal invalidam as aceitação do contrato no idioma correspondente.</span><span class="sxs-lookup"><span data-stu-id="2056d-137">Major version updates invalidate the agreement's acceptances on the corresponding language.</span></span> |
|<span data-ttu-id="2056d-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2056d-138">createdDateTime</span></span>|<span data-ttu-id="2056d-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2056d-139">DateTimeOffset</span></span>|<span data-ttu-id="2056d-140">A data e hora que representam o momento em que o arquivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="2056d-140">The date time representing when the file was created.</span></span> <span data-ttu-id="2056d-141">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2056d-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2056d-142">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="2056d-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|

<!--
## Relationships
| Relationship | Type        | Description |
|:-------------|:------------|:------------|
|localizations|[agreementFileLocalization](agreementfilelocalization.md) collection|The localized version of the agreement files attached to the agreement.|
-->

## <a name="json-representation"></a><span data-ttu-id="2056d-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2056d-143">JSON representation</span></span>

<span data-ttu-id="2056d-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2056d-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFile"
}-->

```json
{
  "fileData": {"@odata.type": "microsoft.graph.agreementFileData"},
  "fileName": "String",
  "id": "String (identifier)",
  "isDefault": true,
  "language": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


