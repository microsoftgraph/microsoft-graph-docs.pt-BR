---
title: tipo de recurso de agreementFile
description: Representa um termos personalizável do arquivo do contrato de uso que gerencia de um inquilino com o Azure Active Directory (AD Azure). Ele contém metadados sobre o arquivo do contrato (por exemplo, o nome, o idioma, e se ele está o arquivo padrão).
ms.openlocfilehash: f099715fd25fbae9d7b2a94d6de841b8766c30e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036943"
---
# <a name="agreementfile-resource-type"></a><span data-ttu-id="d3cf0-104">tipo de recurso de agreementFile</span><span class="sxs-lookup"><span data-stu-id="d3cf0-104">agreementFile resource type</span></span>

> <span data-ttu-id="d3cf0-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d3cf0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3cf0-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d3cf0-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d3cf0-107">Representa um termos personalizável do arquivo do contrato de uso que gerencia de um inquilino com o Azure Active Directory (AD Azure).</span><span class="sxs-lookup"><span data-stu-id="d3cf0-107">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="d3cf0-108">Ele contém metadados sobre o arquivo do contrato (por exemplo, o nome, o idioma, e se ele está o arquivo padrão).</span><span class="sxs-lookup"><span data-stu-id="d3cf0-108">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a><span data-ttu-id="d3cf0-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d3cf0-109">Properties</span></span>
| <span data-ttu-id="d3cf0-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3cf0-110">Property</span></span>     | <span data-ttu-id="d3cf0-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3cf0-111">Type</span></span>        | <span data-ttu-id="d3cf0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3cf0-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d3cf0-113">fileData</span><span class="sxs-lookup"><span data-stu-id="d3cf0-113">fileData</span></span>|[<span data-ttu-id="d3cf0-114">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="d3cf0-114">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="d3cf0-115">Dados que representam as condições de usar o documento PDF.</span><span class="sxs-lookup"><span data-stu-id="d3cf0-115">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="d3cf0-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3cf0-116">Read-only.</span></span>|
|<span data-ttu-id="d3cf0-117">fileName</span><span class="sxs-lookup"><span data-stu-id="d3cf0-117">fileName</span></span>|<span data-ttu-id="d3cf0-118">String</span><span class="sxs-lookup"><span data-stu-id="d3cf0-118">String</span></span>|<span data-ttu-id="d3cf0-119">Nome do arquivo contrato (por exemplo, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="d3cf0-119">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="d3cf0-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3cf0-120">Read-only.</span></span>|
|<span data-ttu-id="d3cf0-121">id</span><span class="sxs-lookup"><span data-stu-id="d3cf0-121">id</span></span>|<span data-ttu-id="d3cf0-122">String</span><span class="sxs-lookup"><span data-stu-id="d3cf0-122">String</span></span>|<span data-ttu-id="d3cf0-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3cf0-123">Read-only.</span></span>|
|<span data-ttu-id="d3cf0-124">isDefault</span><span class="sxs-lookup"><span data-stu-id="d3cf0-124">isDefault</span></span>|<span data-ttu-id="d3cf0-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="d3cf0-125">Boolean</span></span>|<span data-ttu-id="d3cf0-126">Indica se esse é o arquivo padrão do contrato se nenhuma das culturas corresponder a preferência do cliente.</span><span class="sxs-lookup"><span data-stu-id="d3cf0-126">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="d3cf0-127">Se nenhum dos arquivos estiverem marcados como padrão, primeiro será tratado como padrão.</span><span class="sxs-lookup"><span data-stu-id="d3cf0-127">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="d3cf0-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3cf0-128">Read-only.</span></span>|
|<span data-ttu-id="d3cf0-129">idioma</span><span class="sxs-lookup"><span data-stu-id="d3cf0-129">language</span></span>|<span data-ttu-id="d3cf0-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3cf0-130">String</span></span>|<span data-ttu-id="d3cf0-131">Cultura do arquivo no formato languagecode2-país/regioncode2 contrato.</span><span class="sxs-lookup"><span data-stu-id="d3cf0-131">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="d3cf0-132">languagecode2 é um código de duas letras minúsculas, derivado do ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="d3cf0-132">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="d3cf0-133">País/regioncode2 é derivado do ISO 3166 e normalmente consiste em duas letras maiusculas ou uma marca de idioma BCP-47 (por exemplo, en-US).</span><span class="sxs-lookup"><span data-stu-id="d3cf0-133">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="d3cf0-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3cf0-134">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3cf0-135">Relações</span><span class="sxs-lookup"><span data-stu-id="d3cf0-135">Relationships</span></span>
<span data-ttu-id="d3cf0-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d3cf0-136">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="d3cf0-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d3cf0-137">JSON representation</span></span>

<span data-ttu-id="d3cf0-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d3cf0-138">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "agreementFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
