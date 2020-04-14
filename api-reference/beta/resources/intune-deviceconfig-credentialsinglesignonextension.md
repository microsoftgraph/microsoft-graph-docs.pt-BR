---
title: tipo de recurso credentialSingleSignOnExtension
description: Representa um perfil de extensão de logon único de tipo de credencial.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 51c003d84cb323a0fb049be52e46a7d5fce5112b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453468"
---
# <a name="credentialsinglesignonextension-resource-type"></a><span data-ttu-id="ecced-103">tipo de recurso credentialSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="ecced-103">credentialSingleSignOnExtension resource type</span></span>

<span data-ttu-id="ecced-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecced-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ecced-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ecced-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ecced-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ecced-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecced-107">Representa um perfil de extensão de logon único de tipo de credencial.</span><span class="sxs-lookup"><span data-stu-id="ecced-107">Represents a Credential-type Single Sign-On extension profile.</span></span>


<span data-ttu-id="ecced-108">Herda de [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="ecced-108">Inherits from [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ecced-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ecced-109">Properties</span></span>
|<span data-ttu-id="ecced-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ecced-110">Property</span></span>|<span data-ttu-id="ecced-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ecced-111">Type</span></span>|<span data-ttu-id="ecced-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecced-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecced-113">extensionIdentifier</span><span class="sxs-lookup"><span data-stu-id="ecced-113">extensionIdentifier</span></span>|<span data-ttu-id="ecced-114">String</span><span class="sxs-lookup"><span data-stu-id="ecced-114">String</span></span>|<span data-ttu-id="ecced-115">Obtém ou define a ID do pacote da extensão do aplicativo que executa o SSO para as URLs especificadas.</span><span class="sxs-lookup"><span data-stu-id="ecced-115">Gets or sets the bundle ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="ecced-116">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="ecced-116">teamIdentifier</span></span>|<span data-ttu-id="ecced-117">String</span><span class="sxs-lookup"><span data-stu-id="ecced-117">String</span></span>|<span data-ttu-id="ecced-118">Obtém ou define a ID de equipe da extensão de aplicativo que executa o SSO para as URLs especificadas.</span><span class="sxs-lookup"><span data-stu-id="ecced-118">Gets or sets the team ID of the app extension that performs SSO for the specified URLs.</span></span>|
|<span data-ttu-id="ecced-119">domínio</span><span class="sxs-lookup"><span data-stu-id="ecced-119">domains</span></span>|<span data-ttu-id="ecced-120">Coleção String</span><span class="sxs-lookup"><span data-stu-id="ecced-120">String collection</span></span>|<span data-ttu-id="ecced-121">Obtém ou define uma lista de hosts ou nomes de domínio para os quais a extensão de aplicativo executa SSO.</span><span class="sxs-lookup"><span data-stu-id="ecced-121">Gets or sets a list of hosts or domain names for which the app extension performs SSO.</span></span>|
|<span data-ttu-id="ecced-122">esfera</span><span class="sxs-lookup"><span data-stu-id="ecced-122">realm</span></span>|<span data-ttu-id="ecced-123">String</span><span class="sxs-lookup"><span data-stu-id="ecced-123">String</span></span>|<span data-ttu-id="ecced-124">Obtém ou define o nome de território que diferencia maiúsculas de minúsculas para esse perfil.</span><span class="sxs-lookup"><span data-stu-id="ecced-124">Gets or sets the case-sensitive realm name for this profile.</span></span>|
|<span data-ttu-id="ecced-125">as</span><span class="sxs-lookup"><span data-stu-id="ecced-125">configurations</span></span>|<span data-ttu-id="ecced-126">coleção [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="ecced-126">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="ecced-127">Obtém ou define uma lista de pares de valores de chave digitados usados para configurar perfis de tipo de credencial.</span><span class="sxs-lookup"><span data-stu-id="ecced-127">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="ecced-128">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="ecced-128">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ecced-129">Relações</span><span class="sxs-lookup"><span data-stu-id="ecced-129">Relationships</span></span>
<span data-ttu-id="ecced-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ecced-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ecced-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ecced-131">JSON Representation</span></span>
<span data-ttu-id="ecced-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ecced-132">Here is a JSON representation of the resource.</span></span>
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



