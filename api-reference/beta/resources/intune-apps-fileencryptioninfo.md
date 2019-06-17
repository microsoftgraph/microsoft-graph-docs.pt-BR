---
title: Tipo de recurso fileEncryptionInfo
description: Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 725a47eda88cbbdad752d73e6ea3451dcc3d140b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991307"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="fb22c-103">Tipo de recurso fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="fb22c-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="fb22c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fb22c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb22c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fb22c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb22c-106">Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.</span><span class="sxs-lookup"><span data-stu-id="fb22c-106">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="fb22c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fb22c-107">Properties</span></span>
|<span data-ttu-id="fb22c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb22c-108">Property</span></span>|<span data-ttu-id="fb22c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb22c-109">Type</span></span>|<span data-ttu-id="fb22c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb22c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb22c-111">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="fb22c-111">encryptionKey</span></span>|<span data-ttu-id="fb22c-112">Binária</span><span class="sxs-lookup"><span data-stu-id="fb22c-112">Binary</span></span>|<span data-ttu-id="fb22c-113">A chave usada para criptografar o conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="fb22c-113">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="fb22c-114">initializationVector</span><span class="sxs-lookup"><span data-stu-id="fb22c-114">initializationVector</span></span>|<span data-ttu-id="fb22c-115">Binária</span><span class="sxs-lookup"><span data-stu-id="fb22c-115">Binary</span></span>|<span data-ttu-id="fb22c-116">O vetor de inicialização usado para o algoritmo de criptografia.</span><span class="sxs-lookup"><span data-stu-id="fb22c-116">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="fb22c-117">mac</span><span class="sxs-lookup"><span data-stu-id="fb22c-117">mac</span></span>|<span data-ttu-id="fb22c-118">Binária</span><span class="sxs-lookup"><span data-stu-id="fb22c-118">Binary</span></span>|<span data-ttu-id="fb22c-119">O hash do conteúdo do arquivo criptografado + IV (hash conteúdo).</span><span class="sxs-lookup"><span data-stu-id="fb22c-119">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="fb22c-120">macKey</span><span class="sxs-lookup"><span data-stu-id="fb22c-120">macKey</span></span>|<span data-ttu-id="fb22c-121">Binária</span><span class="sxs-lookup"><span data-stu-id="fb22c-121">Binary</span></span>|<span data-ttu-id="fb22c-122">Chave usada para acessar mac.</span><span class="sxs-lookup"><span data-stu-id="fb22c-122">The key used to get mac.</span></span>|
|<span data-ttu-id="fb22c-123">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="fb22c-123">profileIdentifier</span></span>|<span data-ttu-id="fb22c-124">String</span><span class="sxs-lookup"><span data-stu-id="fb22c-124">String</span></span>|<span data-ttu-id="fb22c-125">O identificador de perfil.</span><span class="sxs-lookup"><span data-stu-id="fb22c-125">The the profile identifier.</span></span>|
|<span data-ttu-id="fb22c-126">fileDigest</span><span class="sxs-lookup"><span data-stu-id="fb22c-126">fileDigest</span></span>|<span data-ttu-id="fb22c-127">Binária</span><span class="sxs-lookup"><span data-stu-id="fb22c-127">Binary</span></span>|<span data-ttu-id="fb22c-128">O resumo de arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="fb22c-128">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="fb22c-129">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="fb22c-129">fileDigestAlgorithm</span></span>|<span data-ttu-id="fb22c-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb22c-130">String</span></span>|<span data-ttu-id="fb22c-131">O algoritmo de conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="fb22c-131">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb22c-132">Relações</span><span class="sxs-lookup"><span data-stu-id="fb22c-132">Relationships</span></span>
<span data-ttu-id="fb22c-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fb22c-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb22c-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fb22c-134">JSON Representation</span></span>
<span data-ttu-id="fb22c-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fb22c-135">Here is a JSON representation of the resource.</span></span>
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





