---
title: Tipo de recurso agreementFile
description: Representa um arquivo de contrato de termos de uso personalizável que um locatário gerencia com o Azure Active Directory (Azure AD). Ele contém metadados sobre o arquivo de contrato (por exemplo, o nome, o idioma e se é o arquivo padrão).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: 0c4c84ccdd17be2140d2e72cd0a0c638eef5af6c
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721191"
---
# <a name="agreementfile-resource-type"></a><span data-ttu-id="7b163-104">Tipo de recurso agreementFile</span><span class="sxs-lookup"><span data-stu-id="7b163-104">agreementFile resource type</span></span>

<span data-ttu-id="7b163-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b163-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b163-106">Representa um arquivo de contrato de termos de uso personalizável que um locatário gerencia com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="7b163-106">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="7b163-107">Ele contém metadados sobre o arquivo de contrato (por exemplo, o nome, o idioma e se é o arquivo padrão).</span><span class="sxs-lookup"><span data-stu-id="7b163-107">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a><span data-ttu-id="7b163-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b163-108">Properties</span></span>
| <span data-ttu-id="7b163-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b163-109">Property</span></span>     | <span data-ttu-id="7b163-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b163-110">Type</span></span>        | <span data-ttu-id="7b163-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b163-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7b163-112">fileData</span><span class="sxs-lookup"><span data-stu-id="7b163-112">fileData</span></span>|[<span data-ttu-id="7b163-113">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="7b163-113">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="7b163-114">Dados que representam os termos de uso do documento PDF.</span><span class="sxs-lookup"><span data-stu-id="7b163-114">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="7b163-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7b163-115">Read-only.</span></span>|
|<span data-ttu-id="7b163-116">fileName</span><span class="sxs-lookup"><span data-stu-id="7b163-116">fileName</span></span>|<span data-ttu-id="7b163-117">String</span><span class="sxs-lookup"><span data-stu-id="7b163-117">String</span></span>|<span data-ttu-id="7b163-118">Nome do arquivo de contrato (por exemplo, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="7b163-118">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="7b163-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7b163-119">Read-only.</span></span>|
|<span data-ttu-id="7b163-120">id</span><span class="sxs-lookup"><span data-stu-id="7b163-120">id</span></span>|<span data-ttu-id="7b163-121">String</span><span class="sxs-lookup"><span data-stu-id="7b163-121">String</span></span>|<span data-ttu-id="7b163-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7b163-122">Read-only.</span></span>|
|<span data-ttu-id="7b163-123">isDefault</span><span class="sxs-lookup"><span data-stu-id="7b163-123">isDefault</span></span>|<span data-ttu-id="7b163-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="7b163-124">Boolean</span></span>|<span data-ttu-id="7b163-125">Indica se esse é o arquivo de contrato padrão se nenhuma das culturas corresponde à preferência do cliente.</span><span class="sxs-lookup"><span data-stu-id="7b163-125">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="7b163-126">Se nenhum dos arquivos for marcado como padrão, o primeiro será tratado como padrão.</span><span class="sxs-lookup"><span data-stu-id="7b163-126">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="7b163-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7b163-127">Read-only.</span></span>|
|<span data-ttu-id="7b163-128">idioma</span><span class="sxs-lookup"><span data-stu-id="7b163-128">language</span></span>|<span data-ttu-id="7b163-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7b163-129">String</span></span>|<span data-ttu-id="7b163-130">Cultura do arquivo de contrato no formato languagecode2-country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="7b163-130">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="7b163-131">languagecode2 é um código de duas letras minúsculo derivado da ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="7b163-131">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="7b163-132">country/regioncode2 é derivado da ISO 3166 e geralmente consiste em duas letras maiúsculas, ou uma marca de idioma BCP-47 (por exemplo, en-US).</span><span class="sxs-lookup"><span data-stu-id="7b163-132">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="7b163-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7b163-133">Read-only.</span></span>|
|<span data-ttu-id="7b163-134">isMajorVersion</span><span class="sxs-lookup"><span data-stu-id="7b163-134">isMajorVersion</span></span>|<span data-ttu-id="7b163-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="7b163-135">Boolean</span></span>|<span data-ttu-id="7b163-136">Indica se o arquivo de contrato é uma atualização de versão principal.</span><span class="sxs-lookup"><span data-stu-id="7b163-136">Indicates whether the agreement file is a major version update.</span></span> <span data-ttu-id="7b163-137">Atualizações de versão principais invalidam as aceitaçãos do contrato no idioma correspondente.</span><span class="sxs-lookup"><span data-stu-id="7b163-137">Major version updates invalidate the agreement's acceptances on the corresponding language.</span></span> |
|<span data-ttu-id="7b163-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7b163-138">createdDateTime</span></span>|<span data-ttu-id="7b163-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b163-139">DateTimeOffset</span></span>|<span data-ttu-id="7b163-140">A data que representa quando o arquivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="7b163-140">The date time representing when the file was created.</span></span> <span data-ttu-id="7b163-141">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7b163-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7b163-142">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="7b163-142">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|

<!--
## Relationships
| Relationship | Type        | Description |
|:-------------|:------------|:------------|
|localizations|[agreementFileLocalization](agreementfilelocalization.md) collection|The localized version of the agreement files attached to the agreement.|
-->

## <a name="json-representation"></a><span data-ttu-id="7b163-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b163-143">JSON representation</span></span>

<span data-ttu-id="7b163-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b163-144">The following is a JSON representation of the resource.</span></span>

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


