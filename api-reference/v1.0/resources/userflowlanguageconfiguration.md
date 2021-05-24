---
title: Tipo de recurso userFlowLanguageConfiguration
description: Permite que um fluxo de usuários suporte a vários idiomas.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 556860eb77c4707f1d180b7924ae3126958a4799
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547201"
---
# <a name="userflowlanguageconfiguration-resource-type"></a><span data-ttu-id="9fd18-103">Tipo de recurso userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="9fd18-103">userFlowLanguageConfiguration resource type</span></span>

<span data-ttu-id="9fd18-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fd18-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9fd18-105">Permite que um fluxo de usuários suporte o uso de vários idiomas.</span><span class="sxs-lookup"><span data-stu-id="9fd18-105">Allows a user flow to support the use of multiple languages.</span></span>

<span data-ttu-id="9fd18-106">Para [Azure Active Directory fluxos de usuário](/azure/active-directory/external-identities/user-flow-customize-language), você só pode aproveitar os idiomas integrados fornecidos pela Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9fd18-106">For [Azure Active Directory user flows](/azure/active-directory/external-identities/user-flow-customize-language), you can only leverage the built-in languages provided by Microsoft.</span></span> <span data-ttu-id="9fd18-107">Os fluxos de usuários Azure Active Directory suporte para definir o idioma e as cadeias de caracteres mostradas aos usuários à medida que passam pelas jornadas que você configura com seus fluxos de usuário.</span><span class="sxs-lookup"><span data-stu-id="9fd18-107">User flows for Azure Active Directory support defining the language and strings shown to users as they go through the journeys you configure with your user flows.</span></span>

## <a name="methods"></a><span data-ttu-id="9fd18-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="9fd18-108">Methods</span></span>

|<span data-ttu-id="9fd18-109">Método</span><span class="sxs-lookup"><span data-stu-id="9fd18-109">Method</span></span>|<span data-ttu-id="9fd18-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9fd18-110">Return type</span></span>|<span data-ttu-id="9fd18-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fd18-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9fd18-112">Obter userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="9fd18-112">Get userFlowLanguageConfiguration</span></span>](../api/userflowlanguageconfiguration-get.md)|[<span data-ttu-id="9fd18-113">userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="9fd18-113">userFlowLanguageConfiguration</span></span>](../resources/userflowlanguageconfiguration.md)|<span data-ttu-id="9fd18-114">Leia as propriedades e as relações de um [objeto userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9fd18-114">Read the properties and relationships of a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span> <span data-ttu-id="9fd18-115">Esses objetos representam um idioma disponível em um fluxo de usuários.</span><span class="sxs-lookup"><span data-stu-id="9fd18-115">These objects represent a language available in a user flow.</span></span>|
|[<span data-ttu-id="9fd18-116">Listar defaultPages</span><span class="sxs-lookup"><span data-stu-id="9fd18-116">List defaultPages</span></span>](../api/userflowlanguageconfiguration-list-defaultpages.md)|<span data-ttu-id="9fd18-117">[Coleção userFlowLanguagePage](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="9fd18-117">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="9fd18-118">Obter os recursos userFlowLanguagePage da propriedade de navegação defaultPages.</span><span class="sxs-lookup"><span data-stu-id="9fd18-118">Get the userFlowLanguagePage resources from the defaultPages navigation property.</span></span> <span data-ttu-id="9fd18-119">Representa a jornada padrão do usuário em um fluxo de usuários.</span><span class="sxs-lookup"><span data-stu-id="9fd18-119">Represents the default user journey in a user flow.</span></span>|
|[<span data-ttu-id="9fd18-120">Lista substituiPages</span><span class="sxs-lookup"><span data-stu-id="9fd18-120">List overridesPages</span></span>](../api/userflowlanguageconfiguration-list-overridespages.md)|<span data-ttu-id="9fd18-121">[Coleção userFlowLanguagePage](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="9fd18-121">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="9fd18-122">Obter os recursos userFlowLanguagePage da propriedade de navegação overridesPages.</span><span class="sxs-lookup"><span data-stu-id="9fd18-122">Get the userFlowLanguagePage resources from the overridesPages navigation property.</span></span> <span data-ttu-id="9fd18-123">Representa uma experiência personalizada para uma jornada do usuário em um fluxo de usuários.</span><span class="sxs-lookup"><span data-stu-id="9fd18-123">Represents a custom experience for a user journey in a user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="9fd18-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9fd18-124">Properties</span></span>

|<span data-ttu-id="9fd18-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9fd18-125">Property</span></span>|<span data-ttu-id="9fd18-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fd18-126">Type</span></span>|<span data-ttu-id="9fd18-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fd18-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fd18-128">id</span><span class="sxs-lookup"><span data-stu-id="9fd18-128">id</span></span>|<span data-ttu-id="9fd18-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9fd18-129">String</span></span>|<span data-ttu-id="9fd18-130">O identificador do idioma.</span><span class="sxs-lookup"><span data-stu-id="9fd18-130">The identifier of the language.</span></span> <span data-ttu-id="9fd18-131">Este campo é a marca de identificação de idioma [RFC 5646](https://tools.ietf.org/html/rfc5646) compatível e deve ser uma ID de idioma documentada.</span><span class="sxs-lookup"><span data-stu-id="9fd18-131">This field is Language ID tag [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant and must be a documented Language ID.</span></span>|
|<span data-ttu-id="9fd18-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="9fd18-132">isEnabled</span></span>|<span data-ttu-id="9fd18-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="9fd18-133">Boolean</span></span>|<span data-ttu-id="9fd18-134">Indica se o idioma está habilitado no fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="9fd18-134">Indicates whether the language is enabled within the user flow.</span></span>|
|<span data-ttu-id="9fd18-135">displayName</span><span class="sxs-lookup"><span data-stu-id="9fd18-135">displayName</span></span>|<span data-ttu-id="9fd18-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9fd18-136">String</span></span>|<span data-ttu-id="9fd18-137">O nome do idioma a ser exibido.</span><span class="sxs-lookup"><span data-stu-id="9fd18-137">The language name to display.</span></span> <span data-ttu-id="9fd18-138">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9fd18-138">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fd18-139">Relações</span><span class="sxs-lookup"><span data-stu-id="9fd18-139">Relationships</span></span>

|<span data-ttu-id="9fd18-140">Relação</span><span class="sxs-lookup"><span data-stu-id="9fd18-140">Relationship</span></span>|<span data-ttu-id="9fd18-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fd18-141">Type</span></span>|<span data-ttu-id="9fd18-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fd18-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fd18-143">defaultPages</span><span class="sxs-lookup"><span data-stu-id="9fd18-143">defaultPages</span></span>|<span data-ttu-id="9fd18-144">[Coleção userFlowLanguagePage](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="9fd18-144">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="9fd18-145">Coleção de páginas com o conteúdo padrão a ser exibido em um fluxo de usuário para um idioma especificado.</span><span class="sxs-lookup"><span data-stu-id="9fd18-145">Collection of pages with the default content to display in a user flow for a specified language.</span></span> <span data-ttu-id="9fd18-146">Essa coleção não permite nenhum tipo de modificação.</span><span class="sxs-lookup"><span data-stu-id="9fd18-146">This collection does not allow any kind of modification.</span></span>|
|<span data-ttu-id="9fd18-147">overridesPages</span><span class="sxs-lookup"><span data-stu-id="9fd18-147">overridesPages</span></span>|<span data-ttu-id="9fd18-148">[Coleção userFlowLanguagePage](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="9fd18-148">[userFlowLanguagePage](../resources/userflowlanguagepage.md) collection</span></span>|<span data-ttu-id="9fd18-149">O conjunto de páginas com as mensagens substitui a exibição em um fluxo de usuário para um idioma especificado.</span><span class="sxs-lookup"><span data-stu-id="9fd18-149">Collection of pages with the overrides messages to display in a user flow for a specified language.</span></span> <span data-ttu-id="9fd18-150">Essa coleção só permite modificar o conteúdo da página, qualquer outra modificação não é permitida (criação ou exclusão de páginas).</span><span class="sxs-lookup"><span data-stu-id="9fd18-150">This collection only allows to modify the content of the page, any other modification is not allowed (creation or deletion of pages).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9fd18-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9fd18-151">JSON representation</span></span>

<span data-ttu-id="9fd18-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9fd18-152">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userFlowLanguageConfiguration",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userFlowLanguageConfiguration",
  "id": "String (identifier)",
  "isEnabled": "Boolean",
  "displayName": "String"
}
```
