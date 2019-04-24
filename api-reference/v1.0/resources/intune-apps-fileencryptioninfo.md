---
title: Tipo de recurso fileEncryptionInfo
description: Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 66c4fc3c724eecf3a05dae24cb3f6a52de82d059
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503678"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="87c2f-103">Tipo de recurso fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="87c2f-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="87c2f-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="87c2f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87c2f-105">Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.</span><span class="sxs-lookup"><span data-stu-id="87c2f-105">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="87c2f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87c2f-106">Properties</span></span>
|<span data-ttu-id="87c2f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87c2f-107">Property</span></span>|<span data-ttu-id="87c2f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="87c2f-108">Type</span></span>|<span data-ttu-id="87c2f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="87c2f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87c2f-110">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="87c2f-110">encryptionKey</span></span>|<span data-ttu-id="87c2f-111">Binary</span><span class="sxs-lookup"><span data-stu-id="87c2f-111">Binary</span></span>|<span data-ttu-id="87c2f-112">A chave usada para criptografar o conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="87c2f-112">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="87c2f-113">initializationVector</span><span class="sxs-lookup"><span data-stu-id="87c2f-113">initializationVector</span></span>|<span data-ttu-id="87c2f-114">Binary</span><span class="sxs-lookup"><span data-stu-id="87c2f-114">Binary</span></span>|<span data-ttu-id="87c2f-115">O vetor de inicialização usado para o algoritmo de criptografia.</span><span class="sxs-lookup"><span data-stu-id="87c2f-115">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="87c2f-116">mac</span><span class="sxs-lookup"><span data-stu-id="87c2f-116">mac</span></span>|<span data-ttu-id="87c2f-117">Binary</span><span class="sxs-lookup"><span data-stu-id="87c2f-117">Binary</span></span>|<span data-ttu-id="87c2f-118">O hash do conteúdo do arquivo criptografado + IV (hash conteúdo).</span><span class="sxs-lookup"><span data-stu-id="87c2f-118">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="87c2f-119">macKey</span><span class="sxs-lookup"><span data-stu-id="87c2f-119">macKey</span></span>|<span data-ttu-id="87c2f-120">Binary</span><span class="sxs-lookup"><span data-stu-id="87c2f-120">Binary</span></span>|<span data-ttu-id="87c2f-121">Chave usada para acessar mac.</span><span class="sxs-lookup"><span data-stu-id="87c2f-121">The key used to get mac.</span></span>|
|<span data-ttu-id="87c2f-122">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="87c2f-122">profileIdentifier</span></span>|<span data-ttu-id="87c2f-123">String</span><span class="sxs-lookup"><span data-stu-id="87c2f-123">String</span></span>|<span data-ttu-id="87c2f-124">O identificador de perfil.</span><span class="sxs-lookup"><span data-stu-id="87c2f-124">The the profile identifier.</span></span>|
|<span data-ttu-id="87c2f-125">fileDigest</span><span class="sxs-lookup"><span data-stu-id="87c2f-125">fileDigest</span></span>|<span data-ttu-id="87c2f-126">Binária</span><span class="sxs-lookup"><span data-stu-id="87c2f-126">Binary</span></span>|<span data-ttu-id="87c2f-127">O resumo de arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="87c2f-127">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="87c2f-128">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="87c2f-128">fileDigestAlgorithm</span></span>|<span data-ttu-id="87c2f-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="87c2f-129">String</span></span>|<span data-ttu-id="87c2f-130">O algoritmo de conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="87c2f-130">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87c2f-131">Relações</span><span class="sxs-lookup"><span data-stu-id="87c2f-131">Relationships</span></span>
<span data-ttu-id="87c2f-132">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="87c2f-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="87c2f-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87c2f-133">JSON Representation</span></span>
<span data-ttu-id="87c2f-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="87c2f-134">Here is a JSON representation of the resource.</span></span>
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



