---
title: Tipo de recurso agreementFile
description: Representa um arquivo de contrato de termos de uso personalizável que um locatário gerencia com o Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: fde0912f767510c0c5cd1bf984354099b37be9b0
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722554"
---
# <a name="agreementfile-resource-type"></a><span data-ttu-id="79760-103">Tipo de recurso agreementFile</span><span class="sxs-lookup"><span data-stu-id="79760-103">agreementFile resource type</span></span>

<span data-ttu-id="79760-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79760-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="79760-105">Representa um arquivo de contrato de termos de uso personalizável que um locatário gerencia com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="79760-105">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="79760-106">Ele contém metadados sobre o arquivo de contrato (por exemplo, o nome, o idioma e se é o arquivo padrão).</span><span class="sxs-lookup"><span data-stu-id="79760-106">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

## <a name="properties"></a><span data-ttu-id="79760-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79760-107">Properties</span></span>
| <span data-ttu-id="79760-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79760-108">Property</span></span>     | <span data-ttu-id="79760-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="79760-109">Type</span></span>        | <span data-ttu-id="79760-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="79760-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="79760-111">fileData</span><span class="sxs-lookup"><span data-stu-id="79760-111">fileData</span></span>|[<span data-ttu-id="79760-112">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="79760-112">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="79760-113">Dados que representam os termos de uso do documento PDF.</span><span class="sxs-lookup"><span data-stu-id="79760-113">Data that represents the terms of use PDF document.</span></span> <span data-ttu-id="79760-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="79760-114">Read-only.</span></span>|
|<span data-ttu-id="79760-115">fileName</span><span class="sxs-lookup"><span data-stu-id="79760-115">fileName</span></span>|<span data-ttu-id="79760-116">String</span><span class="sxs-lookup"><span data-stu-id="79760-116">String</span></span>|<span data-ttu-id="79760-117">Nome do arquivo de contrato (por exemplo, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="79760-117">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="79760-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="79760-118">Read-only.</span></span>|
|<span data-ttu-id="79760-119">id</span><span class="sxs-lookup"><span data-stu-id="79760-119">id</span></span>|<span data-ttu-id="79760-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79760-120">String</span></span>|<span data-ttu-id="79760-121">O identificador do arquivo de contrato.</span><span class="sxs-lookup"><span data-stu-id="79760-121">The identifier of the agreement file.</span></span> <span data-ttu-id="79760-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="79760-122">Read-only.</span></span>|
|<span data-ttu-id="79760-123">isDefault</span><span class="sxs-lookup"><span data-stu-id="79760-123">isDefault</span></span>|<span data-ttu-id="79760-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="79760-124">Boolean</span></span>|<span data-ttu-id="79760-125">Se nenhum dos idiomas corresponde à preferência do cliente, indica que esse é o arquivo de contrato padrão.</span><span class="sxs-lookup"><span data-stu-id="79760-125">If none of the languages matches the client preference, indicates that this is the default agreement file.</span></span> <span data-ttu-id="79760-126">Se nenhum dos arquivos for marcado como padrão, o primeiro será tratado como padrão.</span><span class="sxs-lookup"><span data-stu-id="79760-126">If none of the files are marked as default, the first one is treated as the default.</span></span> <span data-ttu-id="79760-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="79760-127">Read-only.</span></span>|
|<span data-ttu-id="79760-128">idioma</span><span class="sxs-lookup"><span data-stu-id="79760-128">language</span></span>|<span data-ttu-id="79760-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79760-129">String</span></span>|<span data-ttu-id="79760-130">O idioma do arquivo de contrato no formato languagecode2-country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="79760-130">The language of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="79760-131">languagecode2 é um código de duas letras minúsculo derivado da ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="79760-131">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="79760-132">country/regioncode2 é derivado da ISO 3166 e geralmente consiste em duas letras maiúsculas, ou uma marca de idioma BCP-47 (por exemplo, en-US).</span><span class="sxs-lookup"><span data-stu-id="79760-132">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="79760-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="79760-133">Read-only.</span></span>|
|<span data-ttu-id="79760-134">isMajorVersion</span><span class="sxs-lookup"><span data-stu-id="79760-134">isMajorVersion</span></span>|<span data-ttu-id="79760-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="79760-135">Boolean</span></span>|<span data-ttu-id="79760-136">Indica se o arquivo de contrato é uma atualização de versão principal.</span><span class="sxs-lookup"><span data-stu-id="79760-136">Indicates whether the agreement file is a major version update.</span></span> <span data-ttu-id="79760-137">Atualizações de versão principais invalidam as aceitaçãos do contrato no idioma correspondente.</span><span class="sxs-lookup"><span data-stu-id="79760-137">Major version updates invalidate the agreement's acceptances on the corresponding language.</span></span> |
|<span data-ttu-id="79760-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79760-138">createdDateTime</span></span>|<span data-ttu-id="79760-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79760-139">DateTimeOffset</span></span>|<span data-ttu-id="79760-140">A data que representa quando o arquivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="79760-140">The date time representing when the file was created.</span></span> <span data-ttu-id="79760-141">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="79760-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="79760-142">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="79760-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|

<!--
## Relationships
| Relationship | Type        | Description |
|:-------------|:------------|:------------|
|localizations|[agreementFileLocalization](agreementfilelocalization.md) collection|The localized version of the agreement files attached to the agreement.|
-->

## <a name="json-representation"></a><span data-ttu-id="79760-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79760-143">JSON representation</span></span>

<span data-ttu-id="79760-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="79760-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.agreementFile",
  "keyProperty": "id"
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


