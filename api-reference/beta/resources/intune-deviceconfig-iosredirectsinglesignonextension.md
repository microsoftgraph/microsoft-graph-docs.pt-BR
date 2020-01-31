---
title: tipo de recurso iosRedirectSingleSignOnExtension
description: Representa um perfil de extensão de logon único de tipo Redirecionado para dispositivos iOS.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 85048bbbdf66166a053be93a124653b17d680a21
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636690"
---
# <a name="iosredirectsinglesignonextension-resource-type"></a><span data-ttu-id="eb7d4-103">tipo de recurso iosRedirectSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="eb7d4-103">iosRedirectSingleSignOnExtension resource type</span></span>

> <span data-ttu-id="eb7d4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eb7d4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb7d4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eb7d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb7d4-106">Representa um perfil de extensão de logon único de tipo Redirecionado para dispositivos iOS.</span><span class="sxs-lookup"><span data-stu-id="eb7d4-106">Represents a Redirect-type Single Sign-On extension profile for iOS devices.</span></span>


<span data-ttu-id="eb7d4-107">Herda de [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="eb7d4-107">Inherits from [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eb7d4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb7d4-108">Properties</span></span>
|<span data-ttu-id="eb7d4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb7d4-109">Property</span></span>|<span data-ttu-id="eb7d4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb7d4-110">Type</span></span>|<span data-ttu-id="eb7d4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb7d4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb7d4-112">extensionIdentifier</span><span class="sxs-lookup"><span data-stu-id="eb7d4-112">extensionIdentifier</span></span>|<span data-ttu-id="eb7d4-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb7d4-113">String</span></span>|<span data-ttu-id="eb7d4-114">Obtém ou define a ID do pacote da extensão do aplicativo que executa o SSO para as URLs especificadas.</span><span class="sxs-lookup"><span data-stu-id="eb7d4-114">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="eb7d4-115">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="eb7d4-115">teamIdentifier</span></span>|<span data-ttu-id="eb7d4-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb7d4-116">String</span></span>|<span data-ttu-id="eb7d4-117">Obtém ou define a ID de equipe da extensão de aplicativo que executa o SSO para as URLs especificadas.</span><span class="sxs-lookup"><span data-stu-id="eb7d4-117">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="eb7d4-118">as</span><span class="sxs-lookup"><span data-stu-id="eb7d4-118">configurations</span></span>|<span data-ttu-id="eb7d4-119">coleção [keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="eb7d4-119">[keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="eb7d4-120">Obtém ou define uma lista de pares de valores de chave digitados usados para configurar perfis de tipo de credencial.</span><span class="sxs-lookup"><span data-stu-id="eb7d4-120">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="eb7d4-121">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="eb7d4-121">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="eb7d4-122">urlPrefixes</span><span class="sxs-lookup"><span data-stu-id="eb7d4-122">urlPrefixes</span></span>|<span data-ttu-id="eb7d4-123">String collection</span><span class="sxs-lookup"><span data-stu-id="eb7d4-123">String collection</span></span>|<span data-ttu-id="eb7d4-124">Um ou mais prefixos de URL de provedores de identidade em cujo nome a extensão do aplicativo executa logon único.</span><span class="sxs-lookup"><span data-stu-id="eb7d4-124">One or more URL prefixes of identity providers on whose behalf the app extension performs single sign-on.</span></span> <span data-ttu-id="eb7d4-125">As URLs devem começar com http://ou https://.</span><span class="sxs-lookup"><span data-stu-id="eb7d4-125">URLs must begin with http:// or https://.</span></span> <span data-ttu-id="eb7d4-126">Todos os prefixos de URL devem ser exclusivos para todos os perfis.</span><span class="sxs-lookup"><span data-stu-id="eb7d4-126">All URL prefixes must be unique for all profiles.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb7d4-127">Relações</span><span class="sxs-lookup"><span data-stu-id="eb7d4-127">Relationships</span></span>
<span data-ttu-id="eb7d4-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eb7d4-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb7d4-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb7d4-129">JSON Representation</span></span>
<span data-ttu-id="eb7d4-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb7d4-130">Here is a JSON representation of the resource.</span></span>
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



