---
title: Tipo de recurso fileEncryptionInfo
description: Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3869a07212d75c002a3a589fd2eda0f6337c8617
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005993"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="f6906-103">Tipo de recurso fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="f6906-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="f6906-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f6906-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6906-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f6906-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6906-106">Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.</span><span class="sxs-lookup"><span data-stu-id="f6906-106">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="f6906-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f6906-107">Properties</span></span>
|<span data-ttu-id="f6906-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f6906-108">Property</span></span>|<span data-ttu-id="f6906-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6906-109">Type</span></span>|<span data-ttu-id="f6906-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6906-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6906-111">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="f6906-111">encryptionKey</span></span>|<span data-ttu-id="f6906-112">Binária</span><span class="sxs-lookup"><span data-stu-id="f6906-112">Binary</span></span>|<span data-ttu-id="f6906-113">A chave usada para criptografar o conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="f6906-113">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="f6906-114">initializationVector</span><span class="sxs-lookup"><span data-stu-id="f6906-114">initializationVector</span></span>|<span data-ttu-id="f6906-115">Binária</span><span class="sxs-lookup"><span data-stu-id="f6906-115">Binary</span></span>|<span data-ttu-id="f6906-116">O vetor de inicialização usado para o algoritmo de criptografia.</span><span class="sxs-lookup"><span data-stu-id="f6906-116">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="f6906-117">mac</span><span class="sxs-lookup"><span data-stu-id="f6906-117">mac</span></span>|<span data-ttu-id="f6906-118">Binária</span><span class="sxs-lookup"><span data-stu-id="f6906-118">Binary</span></span>|<span data-ttu-id="f6906-119">O hash do conteúdo do arquivo criptografado + IV (hash conteúdo).</span><span class="sxs-lookup"><span data-stu-id="f6906-119">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="f6906-120">macKey</span><span class="sxs-lookup"><span data-stu-id="f6906-120">macKey</span></span>|<span data-ttu-id="f6906-121">Binária</span><span class="sxs-lookup"><span data-stu-id="f6906-121">Binary</span></span>|<span data-ttu-id="f6906-122">Chave usada para acessar mac.</span><span class="sxs-lookup"><span data-stu-id="f6906-122">The key used to get mac.</span></span>|
|<span data-ttu-id="f6906-123">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="f6906-123">profileIdentifier</span></span>|<span data-ttu-id="f6906-124">String</span><span class="sxs-lookup"><span data-stu-id="f6906-124">String</span></span>|<span data-ttu-id="f6906-125">O identificador de perfil.</span><span class="sxs-lookup"><span data-stu-id="f6906-125">The the profile identifier.</span></span>|
|<span data-ttu-id="f6906-126">fileDigest</span><span class="sxs-lookup"><span data-stu-id="f6906-126">fileDigest</span></span>|<span data-ttu-id="f6906-127">Binária</span><span class="sxs-lookup"><span data-stu-id="f6906-127">Binary</span></span>|<span data-ttu-id="f6906-128">O resumo de arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="f6906-128">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="f6906-129">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="f6906-129">fileDigestAlgorithm</span></span>|<span data-ttu-id="f6906-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6906-130">String</span></span>|<span data-ttu-id="f6906-131">O algoritmo de conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="f6906-131">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6906-132">Relações</span><span class="sxs-lookup"><span data-stu-id="f6906-132">Relationships</span></span>
<span data-ttu-id="f6906-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f6906-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6906-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f6906-134">JSON Representation</span></span>
<span data-ttu-id="f6906-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f6906-135">Here is a JSON representation of the resource.</span></span>
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





