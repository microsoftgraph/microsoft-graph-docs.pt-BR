---
title: Tipo de recurso fileEncryptionInfo
description: Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3c5586b3107e8b7039df7068d0ab6b00e81bf4b5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42798130"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="3a4a1-103">Tipo de recurso fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="3a4a1-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="3a4a1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3a4a1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a4a1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3a4a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a4a1-106">Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.</span><span class="sxs-lookup"><span data-stu-id="3a4a1-106">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="3a4a1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a4a1-107">Properties</span></span>
|<span data-ttu-id="3a4a1-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a4a1-108">Property</span></span>|<span data-ttu-id="3a4a1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a4a1-109">Type</span></span>|<span data-ttu-id="3a4a1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a4a1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a4a1-111">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="3a4a1-111">encryptionKey</span></span>|<span data-ttu-id="3a4a1-112">Binária</span><span class="sxs-lookup"><span data-stu-id="3a4a1-112">Binary</span></span>|<span data-ttu-id="3a4a1-113">A chave usada para criptografar o conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="3a4a1-113">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="3a4a1-114">initializationVector</span><span class="sxs-lookup"><span data-stu-id="3a4a1-114">initializationVector</span></span>|<span data-ttu-id="3a4a1-115">Binária</span><span class="sxs-lookup"><span data-stu-id="3a4a1-115">Binary</span></span>|<span data-ttu-id="3a4a1-116">O vetor de inicialização usado para o algoritmo de criptografia.</span><span class="sxs-lookup"><span data-stu-id="3a4a1-116">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="3a4a1-117">mac</span><span class="sxs-lookup"><span data-stu-id="3a4a1-117">mac</span></span>|<span data-ttu-id="3a4a1-118">Binária</span><span class="sxs-lookup"><span data-stu-id="3a4a1-118">Binary</span></span>|<span data-ttu-id="3a4a1-119">O hash do conteúdo do arquivo criptografado + IV (hash conteúdo).</span><span class="sxs-lookup"><span data-stu-id="3a4a1-119">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="3a4a1-120">macKey</span><span class="sxs-lookup"><span data-stu-id="3a4a1-120">macKey</span></span>|<span data-ttu-id="3a4a1-121">Binária</span><span class="sxs-lookup"><span data-stu-id="3a4a1-121">Binary</span></span>|<span data-ttu-id="3a4a1-122">Chave usada para acessar mac.</span><span class="sxs-lookup"><span data-stu-id="3a4a1-122">The key used to get mac.</span></span>|
|<span data-ttu-id="3a4a1-123">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="3a4a1-123">profileIdentifier</span></span>|<span data-ttu-id="3a4a1-124">String</span><span class="sxs-lookup"><span data-stu-id="3a4a1-124">String</span></span>|<span data-ttu-id="3a4a1-125">O identificador de perfil.</span><span class="sxs-lookup"><span data-stu-id="3a4a1-125">The the profile identifier.</span></span>|
|<span data-ttu-id="3a4a1-126">fileDigest</span><span class="sxs-lookup"><span data-stu-id="3a4a1-126">fileDigest</span></span>|<span data-ttu-id="3a4a1-127">Binária</span><span class="sxs-lookup"><span data-stu-id="3a4a1-127">Binary</span></span>|<span data-ttu-id="3a4a1-128">O resumo de arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="3a4a1-128">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="3a4a1-129">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="3a4a1-129">fileDigestAlgorithm</span></span>|<span data-ttu-id="3a4a1-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a4a1-130">String</span></span>|<span data-ttu-id="3a4a1-131">O algoritmo de conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="3a4a1-131">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a4a1-132">Relações</span><span class="sxs-lookup"><span data-stu-id="3a4a1-132">Relationships</span></span>
<span data-ttu-id="3a4a1-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3a4a1-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a4a1-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a4a1-134">JSON Representation</span></span>
<span data-ttu-id="3a4a1-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3a4a1-135">Here is a JSON representation of the resource.</span></span>
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



