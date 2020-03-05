---
title: Tipo de recurso fileEncryptionInfo
description: Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5717936692dde3e92071e0f697fa0204bf7550ee
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42493787"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="d1dda-103">Tipo de recurso fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="d1dda-103">fileEncryptionInfo resource type</span></span>

<span data-ttu-id="d1dda-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d1dda-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1dda-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d1dda-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1dda-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d1dda-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1dda-107">Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.</span><span class="sxs-lookup"><span data-stu-id="d1dda-107">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="d1dda-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d1dda-108">Properties</span></span>
|<span data-ttu-id="d1dda-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d1dda-109">Property</span></span>|<span data-ttu-id="d1dda-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1dda-110">Type</span></span>|<span data-ttu-id="d1dda-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1dda-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1dda-112">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="d1dda-112">encryptionKey</span></span>|<span data-ttu-id="d1dda-113">Binária</span><span class="sxs-lookup"><span data-stu-id="d1dda-113">Binary</span></span>|<span data-ttu-id="d1dda-114">A chave usada para criptografar o conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="d1dda-114">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="d1dda-115">initializationVector</span><span class="sxs-lookup"><span data-stu-id="d1dda-115">initializationVector</span></span>|<span data-ttu-id="d1dda-116">Binária</span><span class="sxs-lookup"><span data-stu-id="d1dda-116">Binary</span></span>|<span data-ttu-id="d1dda-117">O vetor de inicialização usado para o algoritmo de criptografia.</span><span class="sxs-lookup"><span data-stu-id="d1dda-117">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="d1dda-118">mac</span><span class="sxs-lookup"><span data-stu-id="d1dda-118">mac</span></span>|<span data-ttu-id="d1dda-119">Binária</span><span class="sxs-lookup"><span data-stu-id="d1dda-119">Binary</span></span>|<span data-ttu-id="d1dda-120">O hash do conteúdo do arquivo criptografado + IV (hash conteúdo).</span><span class="sxs-lookup"><span data-stu-id="d1dda-120">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="d1dda-121">macKey</span><span class="sxs-lookup"><span data-stu-id="d1dda-121">macKey</span></span>|<span data-ttu-id="d1dda-122">Binária</span><span class="sxs-lookup"><span data-stu-id="d1dda-122">Binary</span></span>|<span data-ttu-id="d1dda-123">Chave usada para acessar mac.</span><span class="sxs-lookup"><span data-stu-id="d1dda-123">The key used to get mac.</span></span>|
|<span data-ttu-id="d1dda-124">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="d1dda-124">profileIdentifier</span></span>|<span data-ttu-id="d1dda-125">String</span><span class="sxs-lookup"><span data-stu-id="d1dda-125">String</span></span>|<span data-ttu-id="d1dda-126">O identificador de perfil.</span><span class="sxs-lookup"><span data-stu-id="d1dda-126">The the profile identifier.</span></span>|
|<span data-ttu-id="d1dda-127">fileDigest</span><span class="sxs-lookup"><span data-stu-id="d1dda-127">fileDigest</span></span>|<span data-ttu-id="d1dda-128">Binária</span><span class="sxs-lookup"><span data-stu-id="d1dda-128">Binary</span></span>|<span data-ttu-id="d1dda-129">O resumo de arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="d1dda-129">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="d1dda-130">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="d1dda-130">fileDigestAlgorithm</span></span>|<span data-ttu-id="d1dda-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1dda-131">String</span></span>|<span data-ttu-id="d1dda-132">O algoritmo de conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="d1dda-132">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1dda-133">Relações</span><span class="sxs-lookup"><span data-stu-id="d1dda-133">Relationships</span></span>
<span data-ttu-id="d1dda-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d1dda-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1dda-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d1dda-135">JSON Representation</span></span>
<span data-ttu-id="d1dda-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d1dda-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fileEncryptionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fileEncryptionInfo",
  "encryptionKey": "binary",
  "initializationVector": "binary",
  "mac": "binary",
  "macKey": "binary",
  "profileIdentifier": "String",
  "fileDigest": "binary",
  "fileDigestAlgorithm": "String"
}
```



