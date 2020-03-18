---
title: tipo de recurso credentialSingleSignOnExtension
description: Representa um perfil de extensão de logon único de tipo de credencial.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 72144dc9194f0452b947e2cb72e934893f1721e6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42795656"
---
# <a name="credentialsinglesignonextension-resource-type"></a><span data-ttu-id="f67d8-103">tipo de recurso credentialSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="f67d8-103">credentialSingleSignOnExtension resource type</span></span>

> <span data-ttu-id="f67d8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f67d8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f67d8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f67d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f67d8-106">Representa um perfil de extensão de logon único de tipo de credencial.</span><span class="sxs-lookup"><span data-stu-id="f67d8-106">Represents a Credential-type Single Sign-On extension profile.</span></span>


<span data-ttu-id="f67d8-107">Herda de [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="f67d8-107">Inherits from [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f67d8-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f67d8-108">Properties</span></span>
|<span data-ttu-id="f67d8-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f67d8-109">Property</span></span>|<span data-ttu-id="f67d8-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f67d8-110">Type</span></span>|<span data-ttu-id="f67d8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f67d8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f67d8-112">extensionIdentifier</span><span class="sxs-lookup"><span data-stu-id="f67d8-112">extensionIdentifier</span></span>|<span data-ttu-id="f67d8-113">String</span><span class="sxs-lookup"><span data-stu-id="f67d8-113">String</span></span>|<span data-ttu-id="f67d8-114">Obtém ou define a ID do pacote da extensão do aplicativo que executa o SSO para as URLs especificadas.</span><span class="sxs-lookup"><span data-stu-id="f67d8-114">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="f67d8-115">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="f67d8-115">teamIdentifier</span></span>|<span data-ttu-id="f67d8-116">String</span><span class="sxs-lookup"><span data-stu-id="f67d8-116">String</span></span>|<span data-ttu-id="f67d8-117">Obtém ou define a ID de equipe da extensão de aplicativo que executa o SSO para as URLs especificadas.</span><span class="sxs-lookup"><span data-stu-id="f67d8-117">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="f67d8-118">domínio</span><span class="sxs-lookup"><span data-stu-id="f67d8-118">domains</span></span>|<span data-ttu-id="f67d8-119">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f67d8-119">String collection</span></span>|<span data-ttu-id="f67d8-120">Obtém ou define uma lista de hosts ou nomes de domínio para os quais a extensão de aplicativo executa SSO.</span><span class="sxs-lookup"><span data-stu-id="f67d8-120">Gets or sets a list of hosts or domain names for which the app extension performs SSO.</span></span>|
|<span data-ttu-id="f67d8-121">esfera</span><span class="sxs-lookup"><span data-stu-id="f67d8-121">realm</span></span>|<span data-ttu-id="f67d8-122">String</span><span class="sxs-lookup"><span data-stu-id="f67d8-122">String</span></span>|<span data-ttu-id="f67d8-123">Obtém ou define o nome de território que diferencia maiúsculas de minúsculas para esse perfil.</span><span class="sxs-lookup"><span data-stu-id="f67d8-123">Gets or sets the case-sensitive realm name for this profile.</span></span>|
|<span data-ttu-id="f67d8-124">as</span><span class="sxs-lookup"><span data-stu-id="f67d8-124">configurations</span></span>|<span data-ttu-id="f67d8-125">coleção [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="f67d8-125">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="f67d8-126">Obtém ou define uma lista de pares de valores de chave digitados usados para configurar perfis de tipo de credencial.</span><span class="sxs-lookup"><span data-stu-id="f67d8-126">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="f67d8-127">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="f67d8-127">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f67d8-128">Relações</span><span class="sxs-lookup"><span data-stu-id="f67d8-128">Relationships</span></span>
<span data-ttu-id="f67d8-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f67d8-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f67d8-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f67d8-130">JSON Representation</span></span>
<span data-ttu-id="f67d8-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f67d8-131">Here is a JSON representation of the resource.</span></span>
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



