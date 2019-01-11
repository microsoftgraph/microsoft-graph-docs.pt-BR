---
title: Tipo de recurso fileEncryptionInfo
description: Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ed56f695da8dece64702472cd3822603e02dd8b6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840688"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="07c60-103">Tipo de recurso fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="07c60-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="07c60-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="07c60-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="07c60-105">Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.</span><span class="sxs-lookup"><span data-stu-id="07c60-105">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="07c60-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="07c60-106">Properties</span></span>
|<span data-ttu-id="07c60-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07c60-107">Property</span></span>|<span data-ttu-id="07c60-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="07c60-108">Type</span></span>|<span data-ttu-id="07c60-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="07c60-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07c60-110">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="07c60-110">encryptionKey</span></span>|<span data-ttu-id="07c60-111">Binária</span><span class="sxs-lookup"><span data-stu-id="07c60-111">Binary</span></span>|<span data-ttu-id="07c60-112">A chave usada para criptografar o conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="07c60-112">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="07c60-113">initializationVector</span><span class="sxs-lookup"><span data-stu-id="07c60-113">initializationVector</span></span>|<span data-ttu-id="07c60-114">Binária</span><span class="sxs-lookup"><span data-stu-id="07c60-114">Binary</span></span>|<span data-ttu-id="07c60-115">O vetor de inicialização usado para o algoritmo de criptografia.</span><span class="sxs-lookup"><span data-stu-id="07c60-115">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="07c60-116">mac</span><span class="sxs-lookup"><span data-stu-id="07c60-116">mac</span></span>|<span data-ttu-id="07c60-117">Binária</span><span class="sxs-lookup"><span data-stu-id="07c60-117">Binary</span></span>|<span data-ttu-id="07c60-118">O hash do conteúdo do arquivo criptografado + IV (hash conteúdo).</span><span class="sxs-lookup"><span data-stu-id="07c60-118">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="07c60-119">macKey</span><span class="sxs-lookup"><span data-stu-id="07c60-119">macKey</span></span>|<span data-ttu-id="07c60-120">Binária</span><span class="sxs-lookup"><span data-stu-id="07c60-120">Binary</span></span>|<span data-ttu-id="07c60-121">Chave usada para acessar mac.</span><span class="sxs-lookup"><span data-stu-id="07c60-121">The key used to get mac.</span></span>|
|<span data-ttu-id="07c60-122">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="07c60-122">profileIdentifier</span></span>|<span data-ttu-id="07c60-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07c60-123">String</span></span>|<span data-ttu-id="07c60-124">O identificador de perfil.</span><span class="sxs-lookup"><span data-stu-id="07c60-124">The the profile identifier.</span></span>|
|<span data-ttu-id="07c60-125">fileDigest</span><span class="sxs-lookup"><span data-stu-id="07c60-125">fileDigest</span></span>|<span data-ttu-id="07c60-126">Binária</span><span class="sxs-lookup"><span data-stu-id="07c60-126">Binary</span></span>|<span data-ttu-id="07c60-127">O resumo de arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="07c60-127">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="07c60-128">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="07c60-128">fileDigestAlgorithm</span></span>|<span data-ttu-id="07c60-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07c60-129">String</span></span>|<span data-ttu-id="07c60-130">O algoritmo de conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="07c60-130">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07c60-131">Relações</span><span class="sxs-lookup"><span data-stu-id="07c60-131">Relationships</span></span>
<span data-ttu-id="07c60-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="07c60-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="07c60-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07c60-133">JSON Representation</span></span>
<span data-ttu-id="07c60-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="07c60-134">Here is a JSON representation of the resource.</span></span>
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



