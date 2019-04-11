---
title: Tipo de recurso fileEncryptionInfo
description: Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9a2236e2c63703ea5af2662d5b0f4594e7888799
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789721"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="73ae0-103">Tipo de recurso fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="73ae0-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="73ae0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="73ae0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73ae0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="73ae0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73ae0-106">Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.</span><span class="sxs-lookup"><span data-stu-id="73ae0-106">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="73ae0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="73ae0-107">Properties</span></span>
|<span data-ttu-id="73ae0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73ae0-108">Property</span></span>|<span data-ttu-id="73ae0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="73ae0-109">Type</span></span>|<span data-ttu-id="73ae0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="73ae0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73ae0-111">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="73ae0-111">encryptionKey</span></span>|<span data-ttu-id="73ae0-112">Binary</span><span class="sxs-lookup"><span data-stu-id="73ae0-112">Binary</span></span>|<span data-ttu-id="73ae0-113">A chave usada para criptografar o conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="73ae0-113">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="73ae0-114">initializationVector</span><span class="sxs-lookup"><span data-stu-id="73ae0-114">initializationVector</span></span>|<span data-ttu-id="73ae0-115">Binary</span><span class="sxs-lookup"><span data-stu-id="73ae0-115">Binary</span></span>|<span data-ttu-id="73ae0-116">O vetor de inicialização usado para o algoritmo de criptografia.</span><span class="sxs-lookup"><span data-stu-id="73ae0-116">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="73ae0-117">mac</span><span class="sxs-lookup"><span data-stu-id="73ae0-117">mac</span></span>|<span data-ttu-id="73ae0-118">Binary</span><span class="sxs-lookup"><span data-stu-id="73ae0-118">Binary</span></span>|<span data-ttu-id="73ae0-119">O hash do conteúdo do arquivo criptografado + IV (hash conteúdo).</span><span class="sxs-lookup"><span data-stu-id="73ae0-119">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="73ae0-120">macKey</span><span class="sxs-lookup"><span data-stu-id="73ae0-120">macKey</span></span>|<span data-ttu-id="73ae0-121">Binary</span><span class="sxs-lookup"><span data-stu-id="73ae0-121">Binary</span></span>|<span data-ttu-id="73ae0-122">Chave usada para acessar mac.</span><span class="sxs-lookup"><span data-stu-id="73ae0-122">The key used to get mac.</span></span>|
|<span data-ttu-id="73ae0-123">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="73ae0-123">profileIdentifier</span></span>|<span data-ttu-id="73ae0-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73ae0-124">String</span></span>|<span data-ttu-id="73ae0-125">O identificador de perfil.</span><span class="sxs-lookup"><span data-stu-id="73ae0-125">The the profile identifier.</span></span>|
|<span data-ttu-id="73ae0-126">fileDigest</span><span class="sxs-lookup"><span data-stu-id="73ae0-126">fileDigest</span></span>|<span data-ttu-id="73ae0-127">Binária</span><span class="sxs-lookup"><span data-stu-id="73ae0-127">Binary</span></span>|<span data-ttu-id="73ae0-128">O resumo de arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="73ae0-128">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="73ae0-129">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="73ae0-129">fileDigestAlgorithm</span></span>|<span data-ttu-id="73ae0-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73ae0-130">String</span></span>|<span data-ttu-id="73ae0-131">O algoritmo de conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="73ae0-131">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73ae0-132">Relações</span><span class="sxs-lookup"><span data-stu-id="73ae0-132">Relationships</span></span>
<span data-ttu-id="73ae0-133">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="73ae0-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="73ae0-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="73ae0-134">JSON Representation</span></span>
<span data-ttu-id="73ae0-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="73ae0-135">Here is a JSON representation of the resource.</span></span>
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





