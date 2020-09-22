---
title: tipo de recurso macOSRedirectSingleSignOnExtension
description: Representa um perfil de extensão de logon único de tipo Redirecionado para dispositivos macOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b39d4716909d43430163e0b35213e749df6b1afe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064210"
---
# <a name="macosredirectsinglesignonextension-resource-type"></a><span data-ttu-id="44d17-103">tipo de recurso macOSRedirectSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="44d17-103">macOSRedirectSingleSignOnExtension resource type</span></span>

<span data-ttu-id="44d17-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44d17-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44d17-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="44d17-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44d17-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="44d17-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44d17-107">Representa um perfil de extensão de logon único de tipo Redirecionado para dispositivos macOS.</span><span class="sxs-lookup"><span data-stu-id="44d17-107">Represents a Redirect-type Single Sign-On extension profile for macOS devices.</span></span>


<span data-ttu-id="44d17-108">Herda de [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="44d17-108">Inherits from [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="44d17-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="44d17-109">Properties</span></span>
|<span data-ttu-id="44d17-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44d17-110">Property</span></span>|<span data-ttu-id="44d17-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="44d17-111">Type</span></span>|<span data-ttu-id="44d17-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="44d17-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44d17-113">extensionIdentifier</span><span class="sxs-lookup"><span data-stu-id="44d17-113">extensionIdentifier</span></span>|<span data-ttu-id="44d17-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44d17-114">String</span></span>|<span data-ttu-id="44d17-115">Obtém ou define a ID do pacote da extensão do aplicativo que executa o SSO para as URLs especificadas.</span><span class="sxs-lookup"><span data-stu-id="44d17-115">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="44d17-116">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="44d17-116">teamIdentifier</span></span>|<span data-ttu-id="44d17-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44d17-117">String</span></span>|<span data-ttu-id="44d17-118">Obtém ou define a ID de equipe da extensão de aplicativo que executa o SSO para as URLs especificadas.</span><span class="sxs-lookup"><span data-stu-id="44d17-118">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="44d17-119">as</span><span class="sxs-lookup"><span data-stu-id="44d17-119">configurations</span></span>|<span data-ttu-id="44d17-120">coleção [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="44d17-120">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="44d17-121">Obtém ou define uma lista de pares de valores de chave digitados usados para configurar perfis de tipo de credencial.</span><span class="sxs-lookup"><span data-stu-id="44d17-121">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="44d17-122">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="44d17-122">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="44d17-123">urlPrefixes</span><span class="sxs-lookup"><span data-stu-id="44d17-123">urlPrefixes</span></span>|<span data-ttu-id="44d17-124">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="44d17-124">String collection</span></span>|<span data-ttu-id="44d17-125">Um ou mais prefixos de URL de provedores de identidade em cujo nome a extensão do aplicativo executa logon único.</span><span class="sxs-lookup"><span data-stu-id="44d17-125">One or more URL prefixes of identity providers on whose behalf the app extension performs single sign-on.</span></span> <span data-ttu-id="44d17-126">As URLs devem começar com http://ou https://.</span><span class="sxs-lookup"><span data-stu-id="44d17-126">URLs must begin with http:// or https://.</span></span> <span data-ttu-id="44d17-127">Todos os prefixos de URL devem ser exclusivos para todos os perfis.</span><span class="sxs-lookup"><span data-stu-id="44d17-127">All URL prefixes must be unique for all profiles.</span></span>|

## <a name="relationships"></a><span data-ttu-id="44d17-128">Relações</span><span class="sxs-lookup"><span data-stu-id="44d17-128">Relationships</span></span>
<span data-ttu-id="44d17-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="44d17-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="44d17-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="44d17-130">JSON Representation</span></span>
<span data-ttu-id="44d17-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="44d17-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSRedirectSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSRedirectSingleSignOnExtension",
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






