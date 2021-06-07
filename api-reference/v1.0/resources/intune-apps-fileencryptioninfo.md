---
title: Tipo de recurso fileEncryptionInfo
description: Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7f22c1d25b45b31cf682ad95d573fe3b41534dc9
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755606"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="88fc3-103">Tipo de recurso fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="88fc3-103">fileEncryptionInfo resource type</span></span>

<span data-ttu-id="88fc3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88fc3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88fc3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="88fc3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88fc3-106">Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.</span><span class="sxs-lookup"><span data-stu-id="88fc3-106">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="88fc3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="88fc3-107">Properties</span></span>
|<span data-ttu-id="88fc3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88fc3-108">Property</span></span>|<span data-ttu-id="88fc3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="88fc3-109">Type</span></span>|<span data-ttu-id="88fc3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="88fc3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88fc3-111">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="88fc3-111">encryptionKey</span></span>|<span data-ttu-id="88fc3-112">Binária</span><span class="sxs-lookup"><span data-stu-id="88fc3-112">Binary</span></span>|<span data-ttu-id="88fc3-113">A chave usada para criptografar o conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="88fc3-113">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="88fc3-114">initializationVector</span><span class="sxs-lookup"><span data-stu-id="88fc3-114">initializationVector</span></span>|<span data-ttu-id="88fc3-115">Binária</span><span class="sxs-lookup"><span data-stu-id="88fc3-115">Binary</span></span>|<span data-ttu-id="88fc3-116">O vetor de inicialização usado para o algoritmo de criptografia.</span><span class="sxs-lookup"><span data-stu-id="88fc3-116">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="88fc3-117">mac</span><span class="sxs-lookup"><span data-stu-id="88fc3-117">mac</span></span>|<span data-ttu-id="88fc3-118">Binária</span><span class="sxs-lookup"><span data-stu-id="88fc3-118">Binary</span></span>|<span data-ttu-id="88fc3-119">O hash do conteúdo do arquivo criptografado + IV (hash conteúdo).</span><span class="sxs-lookup"><span data-stu-id="88fc3-119">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="88fc3-120">macKey</span><span class="sxs-lookup"><span data-stu-id="88fc3-120">macKey</span></span>|<span data-ttu-id="88fc3-121">Binária</span><span class="sxs-lookup"><span data-stu-id="88fc3-121">Binary</span></span>|<span data-ttu-id="88fc3-122">Chave usada para acessar mac.</span><span class="sxs-lookup"><span data-stu-id="88fc3-122">The key used to get mac.</span></span>|
|<span data-ttu-id="88fc3-123">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="88fc3-123">profileIdentifier</span></span>|<span data-ttu-id="88fc3-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88fc3-124">String</span></span>|<span data-ttu-id="88fc3-125">O identificador de perfil.</span><span class="sxs-lookup"><span data-stu-id="88fc3-125">The the profile identifier.</span></span>|
|<span data-ttu-id="88fc3-126">fileDigest</span><span class="sxs-lookup"><span data-stu-id="88fc3-126">fileDigest</span></span>|<span data-ttu-id="88fc3-127">Binária</span><span class="sxs-lookup"><span data-stu-id="88fc3-127">Binary</span></span>|<span data-ttu-id="88fc3-128">O resumo de arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="88fc3-128">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="88fc3-129">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="88fc3-129">fileDigestAlgorithm</span></span>|<span data-ttu-id="88fc3-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88fc3-130">String</span></span>|<span data-ttu-id="88fc3-131">O algoritmo de conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="88fc3-131">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88fc3-132">Relações</span><span class="sxs-lookup"><span data-stu-id="88fc3-132">Relationships</span></span>
<span data-ttu-id="88fc3-133">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="88fc3-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="88fc3-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="88fc3-134">JSON Representation</span></span>
<span data-ttu-id="88fc3-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="88fc3-135">Here is a JSON representation of the resource.</span></span>
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




