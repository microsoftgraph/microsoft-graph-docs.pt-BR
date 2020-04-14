---
title: tipo de recurso redirectSingleSignOnExtension
description: Representa uma extensão de logon único da Apple.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3ada6f4561112fdb572e3bf6a7b74eff7a333aae
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449693"
---
# <a name="redirectsinglesignonextension-resource-type"></a><span data-ttu-id="67794-103">tipo de recurso redirectSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="67794-103">redirectSingleSignOnExtension resource type</span></span>

<span data-ttu-id="67794-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67794-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67794-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="67794-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67794-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="67794-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67794-107">Representa uma extensão de logon único da Apple.</span><span class="sxs-lookup"><span data-stu-id="67794-107">Represents an Apple Single Sign-On Extension.</span></span>


<span data-ttu-id="67794-108">Herda de [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="67794-108">Inherits from [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="67794-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="67794-109">Properties</span></span>
|<span data-ttu-id="67794-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67794-110">Property</span></span>|<span data-ttu-id="67794-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="67794-111">Type</span></span>|<span data-ttu-id="67794-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="67794-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67794-113">extensionIdentifier</span><span class="sxs-lookup"><span data-stu-id="67794-113">extensionIdentifier</span></span>|<span data-ttu-id="67794-114">String</span><span class="sxs-lookup"><span data-stu-id="67794-114">String</span></span>|<span data-ttu-id="67794-115">Obtém ou define a ID do pacote da extensão do aplicativo que executa o SSO para as URLs especificadas.</span><span class="sxs-lookup"><span data-stu-id="67794-115">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="67794-116">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="67794-116">teamIdentifier</span></span>|<span data-ttu-id="67794-117">String</span><span class="sxs-lookup"><span data-stu-id="67794-117">String</span></span>|<span data-ttu-id="67794-118">Obtém ou define a ID de equipe da extensão de aplicativo que executa o SSO para as URLs especificadas.</span><span class="sxs-lookup"><span data-stu-id="67794-118">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="67794-119">as</span><span class="sxs-lookup"><span data-stu-id="67794-119">configurations</span></span>|<span data-ttu-id="67794-120">coleção [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="67794-120">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="67794-121">Obtém ou define uma lista de pares de valores de chave digitados usados para configurar perfis de tipo de credencial.</span><span class="sxs-lookup"><span data-stu-id="67794-121">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="67794-122">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="67794-122">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="67794-123">urlPrefixes</span><span class="sxs-lookup"><span data-stu-id="67794-123">urlPrefixes</span></span>|<span data-ttu-id="67794-124">Coleção String</span><span class="sxs-lookup"><span data-stu-id="67794-124">String collection</span></span>|<span data-ttu-id="67794-125">Um ou mais prefixos de URL de provedores de identidade em cujo nome a extensão do aplicativo executa logon único.</span><span class="sxs-lookup"><span data-stu-id="67794-125">One or more URL prefixes of identity providers on whose behalf the app extension performs single sign-on.</span></span> <span data-ttu-id="67794-126">As URLs devem começar com http://ou https://.</span><span class="sxs-lookup"><span data-stu-id="67794-126">URLs must begin with http:// or https://.</span></span> <span data-ttu-id="67794-127">Todos os prefixos de URL devem ser exclusivos para todos os perfis.</span><span class="sxs-lookup"><span data-stu-id="67794-127">All URL prefixes must be unique for all profiles.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67794-128">Relações</span><span class="sxs-lookup"><span data-stu-id="67794-128">Relationships</span></span>
<span data-ttu-id="67794-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="67794-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="67794-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="67794-130">JSON Representation</span></span>
<span data-ttu-id="67794-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="67794-131">Here is a JSON representation of the resource.</span></span>
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



