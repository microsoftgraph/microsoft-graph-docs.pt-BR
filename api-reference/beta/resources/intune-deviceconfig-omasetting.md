---
title: Tipo de recurso omaSetting
description: Configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e05111209d50fec1aee52a5e9ee87baae3ca47a1
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867445"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="63b5f-103">Tipo de recurso omaSetting</span><span class="sxs-lookup"><span data-stu-id="63b5f-103">omaSetting resource type</span></span>

<span data-ttu-id="63b5f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63b5f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63b5f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="63b5f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63b5f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63b5f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63b5f-107">Configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="63b5f-107">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="63b5f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="63b5f-108">Properties</span></span>
|<span data-ttu-id="63b5f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63b5f-109">Property</span></span>|<span data-ttu-id="63b5f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="63b5f-110">Type</span></span>|<span data-ttu-id="63b5f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="63b5f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63b5f-112">displayName</span><span class="sxs-lookup"><span data-stu-id="63b5f-112">displayName</span></span>|<span data-ttu-id="63b5f-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63b5f-113">String</span></span>|<span data-ttu-id="63b5f-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="63b5f-114">Display Name.</span></span>|
|<span data-ttu-id="63b5f-115">description</span><span class="sxs-lookup"><span data-stu-id="63b5f-115">description</span></span>|<span data-ttu-id="63b5f-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63b5f-116">String</span></span>|<span data-ttu-id="63b5f-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="63b5f-117">Description.</span></span>|
|<span data-ttu-id="63b5f-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="63b5f-118">omaUri</span></span>|<span data-ttu-id="63b5f-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63b5f-119">String</span></span>|<span data-ttu-id="63b5f-120">OMA.</span><span class="sxs-lookup"><span data-stu-id="63b5f-120">OMA.</span></span>|
|<span data-ttu-id="63b5f-121">secretReferenceValueId</span><span class="sxs-lookup"><span data-stu-id="63b5f-121">secretReferenceValueId</span></span>|<span data-ttu-id="63b5f-122">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="63b5f-122">String</span></span>|<span data-ttu-id="63b5f-123">ReferenceId para procurar segredo para descriptografia.</span><span class="sxs-lookup"><span data-stu-id="63b5f-123">ReferenceId for looking up secret for decryption.</span></span> <span data-ttu-id="63b5f-124">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="63b5f-124">This property is read-only.</span></span>|
|<span data-ttu-id="63b5f-125">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="63b5f-125">isEncrypted</span></span>|<span data-ttu-id="63b5f-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="63b5f-126">Boolean</span></span>|<span data-ttu-id="63b5f-127">Indica se o campo valor é criptografado.</span><span class="sxs-lookup"><span data-stu-id="63b5f-127">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="63b5f-128">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="63b5f-128">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63b5f-129">Relações</span><span class="sxs-lookup"><span data-stu-id="63b5f-129">Relationships</span></span>
<span data-ttu-id="63b5f-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="63b5f-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="63b5f-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="63b5f-131">JSON Representation</span></span>
<span data-ttu-id="63b5f-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="63b5f-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "secretReferenceValueId": "String",
  "isEncrypted": true
}
```




