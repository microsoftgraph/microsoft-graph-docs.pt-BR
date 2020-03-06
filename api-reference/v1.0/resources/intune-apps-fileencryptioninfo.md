---
title: Tipo de recurso fileEncryptionInfo
description: Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a0859447e06b7264f5018e575c047a283d02dc34
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532844"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="ccade-103">Tipo de recurso fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="ccade-103">fileEncryptionInfo resource type</span></span>

<span data-ttu-id="ccade-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccade-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ccade-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ccade-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccade-106">Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.</span><span class="sxs-lookup"><span data-stu-id="ccade-106">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="ccade-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ccade-107">Properties</span></span>
|<span data-ttu-id="ccade-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ccade-108">Property</span></span>|<span data-ttu-id="ccade-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccade-109">Type</span></span>|<span data-ttu-id="ccade-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccade-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccade-111">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="ccade-111">encryptionKey</span></span>|<span data-ttu-id="ccade-112">Binária</span><span class="sxs-lookup"><span data-stu-id="ccade-112">Binary</span></span>|<span data-ttu-id="ccade-113">A chave usada para criptografar o conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="ccade-113">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="ccade-114">initializationVector</span><span class="sxs-lookup"><span data-stu-id="ccade-114">initializationVector</span></span>|<span data-ttu-id="ccade-115">Binária</span><span class="sxs-lookup"><span data-stu-id="ccade-115">Binary</span></span>|<span data-ttu-id="ccade-116">O vetor de inicialização usado para o algoritmo de criptografia.</span><span class="sxs-lookup"><span data-stu-id="ccade-116">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="ccade-117">mac</span><span class="sxs-lookup"><span data-stu-id="ccade-117">mac</span></span>|<span data-ttu-id="ccade-118">Binária</span><span class="sxs-lookup"><span data-stu-id="ccade-118">Binary</span></span>|<span data-ttu-id="ccade-119">O hash do conteúdo do arquivo criptografado + IV (hash conteúdo).</span><span class="sxs-lookup"><span data-stu-id="ccade-119">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="ccade-120">macKey</span><span class="sxs-lookup"><span data-stu-id="ccade-120">macKey</span></span>|<span data-ttu-id="ccade-121">Binária</span><span class="sxs-lookup"><span data-stu-id="ccade-121">Binary</span></span>|<span data-ttu-id="ccade-122">Chave usada para acessar mac.</span><span class="sxs-lookup"><span data-stu-id="ccade-122">The key used to get mac.</span></span>|
|<span data-ttu-id="ccade-123">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="ccade-123">profileIdentifier</span></span>|<span data-ttu-id="ccade-124">String</span><span class="sxs-lookup"><span data-stu-id="ccade-124">String</span></span>|<span data-ttu-id="ccade-125">O identificador de perfil.</span><span class="sxs-lookup"><span data-stu-id="ccade-125">The profile identifier.</span></span>|
|<span data-ttu-id="ccade-126">fileDigest</span><span class="sxs-lookup"><span data-stu-id="ccade-126">fileDigest</span></span>|<span data-ttu-id="ccade-127">Binária</span><span class="sxs-lookup"><span data-stu-id="ccade-127">Binary</span></span>|<span data-ttu-id="ccade-128">O resumo de arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="ccade-128">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="ccade-129">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="ccade-129">fileDigestAlgorithm</span></span>|<span data-ttu-id="ccade-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ccade-130">String</span></span>|<span data-ttu-id="ccade-131">O algoritmo de conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="ccade-131">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ccade-132">Relações</span><span class="sxs-lookup"><span data-stu-id="ccade-132">Relationships</span></span>
<span data-ttu-id="ccade-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ccade-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ccade-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ccade-134">JSON Representation</span></span>
<span data-ttu-id="ccade-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ccade-135">Here is a JSON representation of the resource.</span></span>
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




