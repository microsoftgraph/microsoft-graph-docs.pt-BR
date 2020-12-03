---
title: tipo de recurso agreementFileLocalization
description: Representa um contrato de arquivos de política localizado de termos de uso no Azure Active Directory (Azure AD). Ele contém metadados sobre o arquivo de contrato (por exemplo, o nome, o idioma e se é o arquivo padrão).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: a3d42d7c4d7b0b2d1d4b107bacf114f86ae6d258
ms.sourcegitcommit: d09d720b56ed6f1fad556e2a3730c2e850db355f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/02/2020
ms.locfileid: "49555634"
---
# <a name="agreementfilelocalization-resource-type"></a><span data-ttu-id="b3044-104">tipo de recurso agreementFileLocalization</span><span class="sxs-lookup"><span data-stu-id="b3044-104">agreementFileLocalization resource type</span></span>

<span data-ttu-id="b3044-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3044-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3044-106">Representa um arquivo de contrato de uso personalizável que um locatário gerencia com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="b3044-106">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="b3044-107">Ele contém metadados sobre o arquivo de contrato (por exemplo, o nome, o idioma e se é o arquivo padrão).</span><span class="sxs-lookup"><span data-stu-id="b3044-107">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Create agreementFileLocalization](../api/agreementfilelocalization-post-agreementfilelocalizations.md) | [agreementfilelocalization](agreementfilelocalization.md) | Create a new agreementFileLocalization. |
| [List agreementFileLocalizations](../api/agreementfilelocalization-list.md) | [agreementfilelocalization](agreementfilelocalization.md) collection | Get an agreementFileLocalization object collection. |
| [Get agreementFileLocalization](../api/agreementfilelocalization-get.md) | [agreementfilelocalization](agreementfilelocalization.md) | Read properties and relationships of an agreementFileLocalization object. |
| [List agreementFileVersions](../api/agreementfileversion-list.md) | [agreementfileversion](agreementfileversion.md) collection | Get an agreementFileVersion object collection. |
| [Get agreementFileVersion](../api/agreementfileversion-get.md) | [agreementfileversion](agreementfileversion.md) | Read properties and relationships of an agreementFileVersion object. |
-->

## <a name="properties"></a><span data-ttu-id="b3044-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b3044-108">Properties</span></span>
| <span data-ttu-id="b3044-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3044-109">Property</span></span>     | <span data-ttu-id="b3044-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3044-110">Type</span></span>        | <span data-ttu-id="b3044-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3044-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b3044-112">fileData</span><span class="sxs-lookup"><span data-stu-id="b3044-112">fileData</span></span>|[<span data-ttu-id="b3044-113">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="b3044-113">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="b3044-114">Dados que representam o documento PDF termos de uso.</span><span class="sxs-lookup"><span data-stu-id="b3044-114">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="b3044-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b3044-115">Read-only.</span></span>|
|<span data-ttu-id="b3044-116">fileName</span><span class="sxs-lookup"><span data-stu-id="b3044-116">fileName</span></span>|<span data-ttu-id="b3044-117">String</span><span class="sxs-lookup"><span data-stu-id="b3044-117">String</span></span>|<span data-ttu-id="b3044-118">Nome do arquivo de contrato (por exemplo, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="b3044-118">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="b3044-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b3044-119">Read-only.</span></span>|
|<span data-ttu-id="b3044-120">id</span><span class="sxs-lookup"><span data-stu-id="b3044-120">id</span></span>|<span data-ttu-id="b3044-121">String</span><span class="sxs-lookup"><span data-stu-id="b3044-121">String</span></span>|<span data-ttu-id="b3044-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b3044-122">Read-only.</span></span>|
|<span data-ttu-id="b3044-123">isDefault</span><span class="sxs-lookup"><span data-stu-id="b3044-123">isDefault</span></span>|<span data-ttu-id="b3044-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3044-124">Boolean</span></span>|<span data-ttu-id="b3044-125">Indica se este é o arquivo de contrato padrão se nenhuma das culturas corresponder à preferência do cliente.</span><span class="sxs-lookup"><span data-stu-id="b3044-125">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="b3044-126">Se nenhum dos arquivos estiver marcado como padrão, o primeiro será tratado como o padrão.</span><span class="sxs-lookup"><span data-stu-id="b3044-126">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="b3044-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b3044-127">Read-only.</span></span>|
|<span data-ttu-id="b3044-128">idioma</span><span class="sxs-lookup"><span data-stu-id="b3044-128">language</span></span>|<span data-ttu-id="b3044-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3044-129">String</span></span>|<span data-ttu-id="b3044-130">Cultura do arquivo de contrato no formato languagecode2-Country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="b3044-130">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="b3044-131">languagecode2 é um código de duas letras em minúsculas derivado de ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="b3044-131">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="b3044-132">Country/regioncode2 é derivado de ISO 3166 e geralmente consiste em duas letras maiúsculas ou uma marca de idioma BCP-47 (por exemplo, en-US).</span><span class="sxs-lookup"><span data-stu-id="b3044-132">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="b3044-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b3044-133">Read-only.</span></span>|
|<span data-ttu-id="b3044-134">isMajorVersion</span><span class="sxs-lookup"><span data-stu-id="b3044-134">isMajorVersion</span></span>|<span data-ttu-id="b3044-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3044-135">Boolean</span></span>|<span data-ttu-id="b3044-136">Indica se o arquivo de contrato é uma atualização de versão principal.</span><span class="sxs-lookup"><span data-stu-id="b3044-136">Indicates whether the agreement file is a major version update.</span></span> <span data-ttu-id="b3044-137">As atualizações de versão principal invalidam as aceitação do contrato no idioma correspondente.</span><span class="sxs-lookup"><span data-stu-id="b3044-137">Major version updates invalidate the agreement's acceptances on the corresponding language.</span></span> |
|<span data-ttu-id="b3044-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3044-138">createdDateTime</span></span>|<span data-ttu-id="b3044-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3044-139">DateTimeOffset</span></span>|<span data-ttu-id="b3044-140">A data e hora que representam o momento em que o arquivo foi criado. O tipo TIMESTAMP representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b3044-140">The date time representing when the file was created.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b3044-141">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="b3044-141">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|

<!--
## Relationships
| Relationship | Type        | Description |
|:-------------|:------------|:------------|
|versions|[agreementFileVersion](agreementfileversion.md) collection|The version history for the localized agreement file.|
-->

## <a name="json-representation"></a><span data-ttu-id="b3044-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b3044-142">JSON representation</span></span>

<span data-ttu-id="b3044-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b3044-143">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFileLocalization"
}-->

```json
{
  "fileData": {"@odata.type": "microsoft.graph.agreementFileData"},
  "fileName": "String",
  "id": "String (identifier)",
  "isDefault": "Boolean",
  "language": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFileLocalization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
