---
title: tipo de recurso macOSRedirectSingleSignOnExtension
description: Representa um perfil de extensão de logon único de tipo Redirecionado para dispositivos macOS.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ba8f2aacd8ffd02a7c0c48274e5da5a4bc22addb
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636019"
---
# <a name="macosredirectsinglesignonextension-resource-type"></a><span data-ttu-id="1a947-103">tipo de recurso macOSRedirectSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="1a947-103">macOSRedirectSingleSignOnExtension resource type</span></span>

> <span data-ttu-id="1a947-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1a947-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a947-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1a947-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a947-106">Representa um perfil de extensão de logon único de tipo Redirecionado para dispositivos macOS.</span><span class="sxs-lookup"><span data-stu-id="1a947-106">Represents a Redirect-type Single Sign-On extension profile for macOS devices.</span></span>


<span data-ttu-id="1a947-107">Herda de [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="1a947-107">Inherits from [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1a947-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a947-108">Properties</span></span>
|<span data-ttu-id="1a947-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a947-109">Property</span></span>|<span data-ttu-id="1a947-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a947-110">Type</span></span>|<span data-ttu-id="1a947-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a947-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a947-112">extensionIdentifier</span><span class="sxs-lookup"><span data-stu-id="1a947-112">extensionIdentifier</span></span>|<span data-ttu-id="1a947-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a947-113">String</span></span>|<span data-ttu-id="1a947-114">Obtém ou define a ID do pacote da extensão do aplicativo que executa o SSO para as URLs especificadas.</span><span class="sxs-lookup"><span data-stu-id="1a947-114">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="1a947-115">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="1a947-115">teamIdentifier</span></span>|<span data-ttu-id="1a947-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a947-116">String</span></span>|<span data-ttu-id="1a947-117">Obtém ou define a ID de equipe da extensão de aplicativo que executa o SSO para as URLs especificadas.</span><span class="sxs-lookup"><span data-stu-id="1a947-117">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="1a947-118">as</span><span class="sxs-lookup"><span data-stu-id="1a947-118">configurations</span></span>|<span data-ttu-id="1a947-119">coleção [keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="1a947-119">[keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="1a947-120">Obtém ou define uma lista de pares de valores de chave digitados usados para configurar perfis de tipo de credencial.</span><span class="sxs-lookup"><span data-stu-id="1a947-120">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="1a947-121">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="1a947-121">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="1a947-122">urlPrefixes</span><span class="sxs-lookup"><span data-stu-id="1a947-122">urlPrefixes</span></span>|<span data-ttu-id="1a947-123">String collection</span><span class="sxs-lookup"><span data-stu-id="1a947-123">String collection</span></span>|<span data-ttu-id="1a947-124">Um ou mais prefixos de URL de provedores de identidade em cujo nome a extensão do aplicativo executa logon único.</span><span class="sxs-lookup"><span data-stu-id="1a947-124">One or more URL prefixes of identity providers on whose behalf the app extension performs single sign-on.</span></span> <span data-ttu-id="1a947-125">As URLs devem começar com http://ou https://.</span><span class="sxs-lookup"><span data-stu-id="1a947-125">URLs must begin with http:// or https://.</span></span> <span data-ttu-id="1a947-126">Todos os prefixos de URL devem ser exclusivos para todos os perfis.</span><span class="sxs-lookup"><span data-stu-id="1a947-126">All URL prefixes must be unique for all profiles.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a947-127">Relações</span><span class="sxs-lookup"><span data-stu-id="1a947-127">Relationships</span></span>
<span data-ttu-id="1a947-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1a947-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a947-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a947-129">JSON Representation</span></span>
<span data-ttu-id="1a947-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1a947-130">Here is a JSON representation of the resource.</span></span>
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



