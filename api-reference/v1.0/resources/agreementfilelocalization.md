---
title: Tipo de recurso agreementFileLocalization
description: Representa um arquivo de política localizado de um contrato de termos de uso no Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 85d5730dda21bec937044d61db0e46dc3473728e
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761881"
---
# <a name="agreementfilelocalization-resource-type"></a><span data-ttu-id="3bf7b-103">Tipo de recurso agreementFileLocalization</span><span class="sxs-lookup"><span data-stu-id="3bf7b-103">agreementFileLocalization resource type</span></span>

<span data-ttu-id="3bf7b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bf7b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3bf7b-105">Representa um arquivo de contrato de termos de uso personalizável que um locatário gerencia com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="3bf7b-105">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="3bf7b-106">Ele contém metadados sobre o arquivo de contrato (por exemplo, o nome, o idioma e se é o arquivo padrão).</span><span class="sxs-lookup"><span data-stu-id="3bf7b-106">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

## <a name="properties"></a><span data-ttu-id="3bf7b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3bf7b-107">Properties</span></span>
| <span data-ttu-id="3bf7b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3bf7b-108">Property</span></span>     | <span data-ttu-id="3bf7b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3bf7b-109">Type</span></span>        | <span data-ttu-id="3bf7b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bf7b-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3bf7b-111">fileData</span><span class="sxs-lookup"><span data-stu-id="3bf7b-111">fileData</span></span>|[<span data-ttu-id="3bf7b-112">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="3bf7b-112">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="3bf7b-113">Dados que representam os termos de uso do documento PDF.</span><span class="sxs-lookup"><span data-stu-id="3bf7b-113">Data that represents the terms of use PDF document.</span></span> <span data-ttu-id="3bf7b-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3bf7b-114">Read-only.</span></span>|
|<span data-ttu-id="3bf7b-115">fileName</span><span class="sxs-lookup"><span data-stu-id="3bf7b-115">fileName</span></span>|<span data-ttu-id="3bf7b-116">String</span><span class="sxs-lookup"><span data-stu-id="3bf7b-116">String</span></span>|<span data-ttu-id="3bf7b-117">Nome do arquivo de contrato (por exemplo, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="3bf7b-117">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="3bf7b-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3bf7b-118">Read-only.</span></span>|
|<span data-ttu-id="3bf7b-119">id</span><span class="sxs-lookup"><span data-stu-id="3bf7b-119">id</span></span>|<span data-ttu-id="3bf7b-120">String</span><span class="sxs-lookup"><span data-stu-id="3bf7b-120">String</span></span>|<span data-ttu-id="3bf7b-121">O identificador do objeto agreementFileLocalization.</span><span class="sxs-lookup"><span data-stu-id="3bf7b-121">The identifier of the agreementFileLocalization object.</span></span> <span data-ttu-id="3bf7b-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3bf7b-122">Read-only.</span></span>|
|<span data-ttu-id="3bf7b-123">isDefault</span><span class="sxs-lookup"><span data-stu-id="3bf7b-123">isDefault</span></span>|<span data-ttu-id="3bf7b-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="3bf7b-124">Boolean</span></span>| <span data-ttu-id="3bf7b-125">Se nenhum dos idiomas corresponde à preferência do cliente, indica que esse é o arquivo de contrato padrão.</span><span class="sxs-lookup"><span data-stu-id="3bf7b-125">If none of the languages matches the client preference, indicates that this is the default agreement file.</span></span> <span data-ttu-id="3bf7b-126">Se nenhum dos arquivos for marcado como padrão, o primeiro será tratado como padrão.</span><span class="sxs-lookup"><span data-stu-id="3bf7b-126">If none of the files are marked as default, the first one is treated as the default.</span></span> <span data-ttu-id="3bf7b-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3bf7b-127">Read-only.</span></span>|
|<span data-ttu-id="3bf7b-128">idioma</span><span class="sxs-lookup"><span data-stu-id="3bf7b-128">language</span></span>|<span data-ttu-id="3bf7b-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3bf7b-129">String</span></span>|<span data-ttu-id="3bf7b-130">O idioma do arquivo de contrato no formato languagecode2-country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="3bf7b-130">The language of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="3bf7b-131">languagecode2 é um código de duas letras minúsculo derivado da ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="3bf7b-131">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="3bf7b-132">country/regioncode2 é derivado da ISO 3166 e geralmente consiste em duas letras maiúsculas, ou uma marca de idioma BCP-47 (por exemplo, en-US).</span><span class="sxs-lookup"><span data-stu-id="3bf7b-132">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="3bf7b-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3bf7b-133">Read-only.</span></span>|
|<span data-ttu-id="3bf7b-134">isMajorVersion</span><span class="sxs-lookup"><span data-stu-id="3bf7b-134">isMajorVersion</span></span>|<span data-ttu-id="3bf7b-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="3bf7b-135">Boolean</span></span>|<span data-ttu-id="3bf7b-136">Indica se o arquivo de contrato é uma atualização de versão principal.</span><span class="sxs-lookup"><span data-stu-id="3bf7b-136">Indicates whether the agreement file is a major version update.</span></span> <span data-ttu-id="3bf7b-137">Atualizações de versão principais invalidam as aceitaçãos do contrato no idioma correspondente.</span><span class="sxs-lookup"><span data-stu-id="3bf7b-137">Major version updates invalidate the agreement's acceptances on the corresponding language.</span></span> |
|<span data-ttu-id="3bf7b-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3bf7b-138">createdDateTime</span></span>|<span data-ttu-id="3bf7b-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bf7b-139">DateTimeOffset</span></span>|<span data-ttu-id="3bf7b-140">A data que representa quando o arquivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="3bf7b-140">The date time representing when the file was created.</span></span> <span data-ttu-id="3bf7b-141">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="3bf7b-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3bf7b-142">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="3bf7b-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="3bf7b-143">displayName</span><span class="sxs-lookup"><span data-stu-id="3bf7b-143">displayName</span></span>|<span data-ttu-id="3bf7b-144">String</span><span class="sxs-lookup"><span data-stu-id="3bf7b-144">String</span></span>|<span data-ttu-id="3bf7b-145">Nome de exibição localizado do arquivo de política de um contrato.</span><span class="sxs-lookup"><span data-stu-id="3bf7b-145">Localized display name of the policy file of an agreement.</span></span> <span data-ttu-id="3bf7b-146">O nome de exibição localizado é mostrado aos usuários finais que visualizam o contrato.</span><span class="sxs-lookup"><span data-stu-id="3bf7b-146">The localized display name is shown to end users who view the agreement.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3bf7b-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3bf7b-147">JSON representation</span></span>

<span data-ttu-id="3bf7b-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3bf7b-148">The following is a JSON representation of the resource.</span></span>

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
