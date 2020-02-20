---
title: tipo de recurso redirectSingleSignOnExtension
description: Representa uma extensão de logon único da Apple.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7d789df2973d673df32dc66e60ca60d085b8b2ae
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42163791"
---
# <a name="redirectsinglesignonextension-resource-type"></a><span data-ttu-id="24b80-103">tipo de recurso redirectSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="24b80-103">redirectSingleSignOnExtension resource type</span></span>

> <span data-ttu-id="24b80-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="24b80-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24b80-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="24b80-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24b80-106">Representa uma extensão de logon único da Apple.</span><span class="sxs-lookup"><span data-stu-id="24b80-106">Represents an Apple Single Sign-On Extension.</span></span>


<span data-ttu-id="24b80-107">Herda de [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="24b80-107">Inherits from [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="24b80-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="24b80-108">Properties</span></span>
|<span data-ttu-id="24b80-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="24b80-109">Property</span></span>|<span data-ttu-id="24b80-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="24b80-110">Type</span></span>|<span data-ttu-id="24b80-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="24b80-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24b80-112">extensionIdentifier</span><span class="sxs-lookup"><span data-stu-id="24b80-112">extensionIdentifier</span></span>|<span data-ttu-id="24b80-113">String</span><span class="sxs-lookup"><span data-stu-id="24b80-113">String</span></span>|<span data-ttu-id="24b80-114">Obtém ou define a ID do pacote da extensão do aplicativo que executa o SSO para as URLs especificadas.</span><span class="sxs-lookup"><span data-stu-id="24b80-114">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="24b80-115">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="24b80-115">teamIdentifier</span></span>|<span data-ttu-id="24b80-116">String</span><span class="sxs-lookup"><span data-stu-id="24b80-116">String</span></span>|<span data-ttu-id="24b80-117">Obtém ou define a ID de equipe da extensão de aplicativo que executa o SSO para as URLs especificadas.</span><span class="sxs-lookup"><span data-stu-id="24b80-117">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="24b80-118">as</span><span class="sxs-lookup"><span data-stu-id="24b80-118">configurations</span></span>|<span data-ttu-id="24b80-119">coleção [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="24b80-119">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="24b80-120">Obtém ou define uma lista de pares de valores de chave digitados usados para configurar perfis de tipo de credencial.</span><span class="sxs-lookup"><span data-stu-id="24b80-120">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="24b80-121">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="24b80-121">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="24b80-122">urlPrefixes</span><span class="sxs-lookup"><span data-stu-id="24b80-122">urlPrefixes</span></span>|<span data-ttu-id="24b80-123">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="24b80-123">String collection</span></span>|<span data-ttu-id="24b80-124">Um ou mais prefixos de URL de provedores de identidade em cujo nome a extensão do aplicativo executa logon único.</span><span class="sxs-lookup"><span data-stu-id="24b80-124">One or more URL prefixes of identity providers on whose behalf the app extension performs single sign-on.</span></span> <span data-ttu-id="24b80-125">As URLs devem começar com http://ou https://.</span><span class="sxs-lookup"><span data-stu-id="24b80-125">URLs must begin with http:// or https://.</span></span> <span data-ttu-id="24b80-126">Todos os prefixos de URL devem ser exclusivos para todos os perfis.</span><span class="sxs-lookup"><span data-stu-id="24b80-126">All URL prefixes must be unique for all profiles.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24b80-127">Relações</span><span class="sxs-lookup"><span data-stu-id="24b80-127">Relationships</span></span>
<span data-ttu-id="24b80-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="24b80-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24b80-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="24b80-129">JSON Representation</span></span>
<span data-ttu-id="24b80-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="24b80-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.redirectSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.redirectSingleSignOnExtension",
  "extensionIdentifier": "String",
  "teamIdentifier": "String",
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyStringValuePair",
      "key": "String",
      "value": "String"
    }
  ],
  "urlPrefixes": [
    "String"
  ]
}
```



