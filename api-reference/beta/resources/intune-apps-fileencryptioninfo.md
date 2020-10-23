---
title: Tipo de recurso fileEncryptionInfo
description: Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 014e455ac0fed4e6878ab1de55ff1dff35559b98
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730774"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="9a2f3-103">Tipo de recurso fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="9a2f3-103">fileEncryptionInfo resource type</span></span>

<span data-ttu-id="9a2f3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a2f3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a2f3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9a2f3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a2f3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9a2f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a2f3-107">Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.</span><span class="sxs-lookup"><span data-stu-id="9a2f3-107">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="9a2f3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9a2f3-108">Properties</span></span>
|<span data-ttu-id="9a2f3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a2f3-109">Property</span></span>|<span data-ttu-id="9a2f3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a2f3-110">Type</span></span>|<span data-ttu-id="9a2f3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a2f3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a2f3-112">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="9a2f3-112">encryptionKey</span></span>|<span data-ttu-id="9a2f3-113">Binária</span><span class="sxs-lookup"><span data-stu-id="9a2f3-113">Binary</span></span>|<span data-ttu-id="9a2f3-114">A chave usada para criptografar o conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="9a2f3-114">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="9a2f3-115">initializationVector</span><span class="sxs-lookup"><span data-stu-id="9a2f3-115">initializationVector</span></span>|<span data-ttu-id="9a2f3-116">Binária</span><span class="sxs-lookup"><span data-stu-id="9a2f3-116">Binary</span></span>|<span data-ttu-id="9a2f3-117">O vetor de inicialização usado para o algoritmo de criptografia.</span><span class="sxs-lookup"><span data-stu-id="9a2f3-117">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="9a2f3-118">mac</span><span class="sxs-lookup"><span data-stu-id="9a2f3-118">mac</span></span>|<span data-ttu-id="9a2f3-119">Binária</span><span class="sxs-lookup"><span data-stu-id="9a2f3-119">Binary</span></span>|<span data-ttu-id="9a2f3-120">O hash do conteúdo do arquivo criptografado + IV (hash conteúdo).</span><span class="sxs-lookup"><span data-stu-id="9a2f3-120">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="9a2f3-121">macKey</span><span class="sxs-lookup"><span data-stu-id="9a2f3-121">macKey</span></span>|<span data-ttu-id="9a2f3-122">Binária</span><span class="sxs-lookup"><span data-stu-id="9a2f3-122">Binary</span></span>|<span data-ttu-id="9a2f3-123">Chave usada para acessar mac.</span><span class="sxs-lookup"><span data-stu-id="9a2f3-123">The key used to get mac.</span></span>|
|<span data-ttu-id="9a2f3-124">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="9a2f3-124">profileIdentifier</span></span>|<span data-ttu-id="9a2f3-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a2f3-125">String</span></span>|<span data-ttu-id="9a2f3-126">O identificador de perfil.</span><span class="sxs-lookup"><span data-stu-id="9a2f3-126">The the profile identifier.</span></span>|
|<span data-ttu-id="9a2f3-127">fileDigest</span><span class="sxs-lookup"><span data-stu-id="9a2f3-127">fileDigest</span></span>|<span data-ttu-id="9a2f3-128">Binária</span><span class="sxs-lookup"><span data-stu-id="9a2f3-128">Binary</span></span>|<span data-ttu-id="9a2f3-129">O resumo de arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="9a2f3-129">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="9a2f3-130">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="9a2f3-130">fileDigestAlgorithm</span></span>|<span data-ttu-id="9a2f3-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a2f3-131">String</span></span>|<span data-ttu-id="9a2f3-132">O algoritmo de conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="9a2f3-132">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a2f3-133">Relações</span><span class="sxs-lookup"><span data-stu-id="9a2f3-133">Relationships</span></span>
<span data-ttu-id="9a2f3-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9a2f3-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a2f3-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9a2f3-135">JSON Representation</span></span>
<span data-ttu-id="9a2f3-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9a2f3-136">Here is a JSON representation of the resource.</span></span>
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





