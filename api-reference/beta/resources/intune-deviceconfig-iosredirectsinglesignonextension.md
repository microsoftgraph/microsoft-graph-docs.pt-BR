---
title: tipo de recurso iosRedirectSingleSignOnExtension
description: Representa um perfil de extensão de logon único de tipo Redirecionado para dispositivos iOS.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0bcff1697c8d41889736cbe74039f8c43d53d680
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790556"
---
# <a name="iosredirectsinglesignonextension-resource-type"></a><span data-ttu-id="eda84-103">tipo de recurso iosRedirectSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="eda84-103">iosRedirectSingleSignOnExtension resource type</span></span>

> <span data-ttu-id="eda84-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eda84-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eda84-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eda84-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eda84-106">Representa um perfil de extensão de logon único de tipo Redirecionado para dispositivos iOS.</span><span class="sxs-lookup"><span data-stu-id="eda84-106">Represents a Redirect-type Single Sign-On extension profile for iOS devices.</span></span>


<span data-ttu-id="eda84-107">Herda de [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="eda84-107">Inherits from [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eda84-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eda84-108">Properties</span></span>
|<span data-ttu-id="eda84-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eda84-109">Property</span></span>|<span data-ttu-id="eda84-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="eda84-110">Type</span></span>|<span data-ttu-id="eda84-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="eda84-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eda84-112">extensionIdentifier</span><span class="sxs-lookup"><span data-stu-id="eda84-112">extensionIdentifier</span></span>|<span data-ttu-id="eda84-113">String</span><span class="sxs-lookup"><span data-stu-id="eda84-113">String</span></span>|<span data-ttu-id="eda84-114">Obtém ou define a ID do pacote da extensão do aplicativo que executa o SSO para as URLs especificadas.</span><span class="sxs-lookup"><span data-stu-id="eda84-114">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="eda84-115">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="eda84-115">teamIdentifier</span></span>|<span data-ttu-id="eda84-116">String</span><span class="sxs-lookup"><span data-stu-id="eda84-116">String</span></span>|<span data-ttu-id="eda84-117">Obtém ou define a ID de equipe da extensão de aplicativo que executa o SSO para as URLs especificadas.</span><span class="sxs-lookup"><span data-stu-id="eda84-117">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="eda84-118">as</span><span class="sxs-lookup"><span data-stu-id="eda84-118">configurations</span></span>|<span data-ttu-id="eda84-119">coleção [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="eda84-119">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="eda84-120">Obtém ou define uma lista de pares de valores de chave digitados usados para configurar perfis de tipo de credencial.</span><span class="sxs-lookup"><span data-stu-id="eda84-120">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="eda84-121">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="eda84-121">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="eda84-122">urlPrefixes</span><span class="sxs-lookup"><span data-stu-id="eda84-122">urlPrefixes</span></span>|<span data-ttu-id="eda84-123">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="eda84-123">String collection</span></span>|<span data-ttu-id="eda84-124">Um ou mais prefixos de URL de provedores de identidade em cujo nome a extensão do aplicativo executa logon único.</span><span class="sxs-lookup"><span data-stu-id="eda84-124">One or more URL prefixes of identity providers on whose behalf the app extension performs single sign-on.</span></span> <span data-ttu-id="eda84-125">As URLs devem começar com http://ou https://.</span><span class="sxs-lookup"><span data-stu-id="eda84-125">URLs must begin with http:// or https://.</span></span> <span data-ttu-id="eda84-126">Todos os prefixos de URL devem ser exclusivos para todos os perfis.</span><span class="sxs-lookup"><span data-stu-id="eda84-126">All URL prefixes must be unique for all profiles.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eda84-127">Relações</span><span class="sxs-lookup"><span data-stu-id="eda84-127">Relationships</span></span>
<span data-ttu-id="eda84-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eda84-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eda84-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eda84-129">JSON Representation</span></span>
<span data-ttu-id="eda84-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eda84-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosRedirectSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosRedirectSingleSignOnExtension",
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



