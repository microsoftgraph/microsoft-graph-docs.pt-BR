---
title: tipo de recurso credentialSingleSignOnExtension
description: Representa um perfil de extensão de logon único de tipo de credencial.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 588dc5e92a46e7361ca083570a4b92d0f3fbff62
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199697"
---
# <a name="credentialsinglesignonextension-resource-type"></a><span data-ttu-id="57039-103">tipo de recurso credentialSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="57039-103">credentialSingleSignOnExtension resource type</span></span>

> <span data-ttu-id="57039-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="57039-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57039-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="57039-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57039-106">Representa um perfil de extensão de logon único de tipo de credencial.</span><span class="sxs-lookup"><span data-stu-id="57039-106">Represents a Credential-type Single Sign-On extension profile.</span></span>


<span data-ttu-id="57039-107">Herda de [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="57039-107">Inherits from [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="57039-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="57039-108">Properties</span></span>
|<span data-ttu-id="57039-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57039-109">Property</span></span>|<span data-ttu-id="57039-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="57039-110">Type</span></span>|<span data-ttu-id="57039-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="57039-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57039-112">extensionIdentifier</span><span class="sxs-lookup"><span data-stu-id="57039-112">extensionIdentifier</span></span>|<span data-ttu-id="57039-113">String</span><span class="sxs-lookup"><span data-stu-id="57039-113">String</span></span>|<span data-ttu-id="57039-114">Obtém ou define a ID do pacote da extensão do aplicativo que executa o SSO para as URLs especificadas.</span><span class="sxs-lookup"><span data-stu-id="57039-114">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="57039-115">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="57039-115">teamIdentifier</span></span>|<span data-ttu-id="57039-116">String</span><span class="sxs-lookup"><span data-stu-id="57039-116">String</span></span>|<span data-ttu-id="57039-117">Obtém ou define a ID de equipe da extensão de aplicativo que executa o SSO para as URLs especificadas.</span><span class="sxs-lookup"><span data-stu-id="57039-117">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="57039-118">domínio</span><span class="sxs-lookup"><span data-stu-id="57039-118">domains</span></span>|<span data-ttu-id="57039-119">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="57039-119">String collection</span></span>|<span data-ttu-id="57039-120">Obtém ou define uma lista de hosts ou nomes de domínio para os quais a extensão de aplicativo executa SSO.</span><span class="sxs-lookup"><span data-stu-id="57039-120">Gets or sets a list of hosts or domain names for which the app extension performs SSO.</span></span>|
|<span data-ttu-id="57039-121">esfera</span><span class="sxs-lookup"><span data-stu-id="57039-121">realm</span></span>|<span data-ttu-id="57039-122">String</span><span class="sxs-lookup"><span data-stu-id="57039-122">String</span></span>|<span data-ttu-id="57039-123">Obtém ou define o nome de território que diferencia maiúsculas de minúsculas para esse perfil.</span><span class="sxs-lookup"><span data-stu-id="57039-123">Gets or sets the case-sensitive realm name for this profile.</span></span>|
|<span data-ttu-id="57039-124">as</span><span class="sxs-lookup"><span data-stu-id="57039-124">configurations</span></span>|<span data-ttu-id="57039-125">coleção [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="57039-125">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="57039-126">Obtém ou define uma lista de pares de valores de chave digitados usados para configurar perfis de tipo de credencial.</span><span class="sxs-lookup"><span data-stu-id="57039-126">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="57039-127">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="57039-127">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="57039-128">Relações</span><span class="sxs-lookup"><span data-stu-id="57039-128">Relationships</span></span>
<span data-ttu-id="57039-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="57039-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="57039-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="57039-130">JSON Representation</span></span>
<span data-ttu-id="57039-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="57039-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.credentialSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.credentialSingleSignOnExtension",
  "extensionIdentifier": "String",
  "teamIdentifier": "String",
  "domains": [
    "String"
  ],
  "realm": "String",
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyStringValuePair",
      "key": "String",
      "value": "String"
    }
  ]
}
```



