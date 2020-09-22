---
title: Tipo de recurso fileEncryptionInfo
description: Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7c020aa549e9e9a7c2520db6893d0cc60f65b8a1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988279"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="8434a-103">Tipo de recurso fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="8434a-103">fileEncryptionInfo resource type</span></span>

<span data-ttu-id="8434a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8434a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8434a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8434a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8434a-106">Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.</span><span class="sxs-lookup"><span data-stu-id="8434a-106">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="8434a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8434a-107">Properties</span></span>
|<span data-ttu-id="8434a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8434a-108">Property</span></span>|<span data-ttu-id="8434a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8434a-109">Type</span></span>|<span data-ttu-id="8434a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8434a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8434a-111">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="8434a-111">encryptionKey</span></span>|<span data-ttu-id="8434a-112">Binária</span><span class="sxs-lookup"><span data-stu-id="8434a-112">Binary</span></span>|<span data-ttu-id="8434a-113">A chave usada para criptografar o conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="8434a-113">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="8434a-114">initializationVector</span><span class="sxs-lookup"><span data-stu-id="8434a-114">initializationVector</span></span>|<span data-ttu-id="8434a-115">Binária</span><span class="sxs-lookup"><span data-stu-id="8434a-115">Binary</span></span>|<span data-ttu-id="8434a-116">O vetor de inicialização usado para o algoritmo de criptografia.</span><span class="sxs-lookup"><span data-stu-id="8434a-116">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="8434a-117">mac</span><span class="sxs-lookup"><span data-stu-id="8434a-117">mac</span></span>|<span data-ttu-id="8434a-118">Binária</span><span class="sxs-lookup"><span data-stu-id="8434a-118">Binary</span></span>|<span data-ttu-id="8434a-119">O hash do conteúdo do arquivo criptografado + IV (hash conteúdo).</span><span class="sxs-lookup"><span data-stu-id="8434a-119">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="8434a-120">macKey</span><span class="sxs-lookup"><span data-stu-id="8434a-120">macKey</span></span>|<span data-ttu-id="8434a-121">Binária</span><span class="sxs-lookup"><span data-stu-id="8434a-121">Binary</span></span>|<span data-ttu-id="8434a-122">Chave usada para acessar mac.</span><span class="sxs-lookup"><span data-stu-id="8434a-122">The key used to get mac.</span></span>|
|<span data-ttu-id="8434a-123">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="8434a-123">profileIdentifier</span></span>|<span data-ttu-id="8434a-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8434a-124">String</span></span>|<span data-ttu-id="8434a-125">O identificador de perfil.</span><span class="sxs-lookup"><span data-stu-id="8434a-125">The profile identifier.</span></span>|
|<span data-ttu-id="8434a-126">fileDigest</span><span class="sxs-lookup"><span data-stu-id="8434a-126">fileDigest</span></span>|<span data-ttu-id="8434a-127">Binária</span><span class="sxs-lookup"><span data-stu-id="8434a-127">Binary</span></span>|<span data-ttu-id="8434a-128">O resumo de arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="8434a-128">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="8434a-129">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="8434a-129">fileDigestAlgorithm</span></span>|<span data-ttu-id="8434a-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8434a-130">String</span></span>|<span data-ttu-id="8434a-131">O algoritmo de conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="8434a-131">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8434a-132">Relações</span><span class="sxs-lookup"><span data-stu-id="8434a-132">Relationships</span></span>
<span data-ttu-id="8434a-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8434a-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8434a-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8434a-134">JSON Representation</span></span>
<span data-ttu-id="8434a-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8434a-135">Here is a JSON representation of the resource.</span></span>
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









