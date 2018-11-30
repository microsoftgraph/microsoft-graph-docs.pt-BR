---
title: Tipo de recurso fileEncryptionInfo
description: Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.
ms.openlocfilehash: 92aceaa56221287dcde67dcefb4d9ae7109d9273
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006867"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="47f54-103">Tipo de recurso fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="47f54-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="47f54-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="47f54-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47f54-105">Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.</span><span class="sxs-lookup"><span data-stu-id="47f54-105">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="47f54-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="47f54-106">Properties</span></span>
|<span data-ttu-id="47f54-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47f54-107">Property</span></span>|<span data-ttu-id="47f54-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="47f54-108">Type</span></span>|<span data-ttu-id="47f54-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="47f54-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47f54-110">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="47f54-110">encryptionKey</span></span>|<span data-ttu-id="47f54-111">Binária</span><span class="sxs-lookup"><span data-stu-id="47f54-111">Binary</span></span>|<span data-ttu-id="47f54-112">A chave usada para criptografar o conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="47f54-112">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="47f54-113">initializationVector</span><span class="sxs-lookup"><span data-stu-id="47f54-113">initializationVector</span></span>|<span data-ttu-id="47f54-114">Binária</span><span class="sxs-lookup"><span data-stu-id="47f54-114">Binary</span></span>|<span data-ttu-id="47f54-115">O vetor de inicialização usado para o algoritmo de criptografia.</span><span class="sxs-lookup"><span data-stu-id="47f54-115">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="47f54-116">mac</span><span class="sxs-lookup"><span data-stu-id="47f54-116">mac</span></span>|<span data-ttu-id="47f54-117">Binária</span><span class="sxs-lookup"><span data-stu-id="47f54-117">Binary</span></span>|<span data-ttu-id="47f54-118">O hash do conteúdo do arquivo criptografado + IV (hash conteúdo).</span><span class="sxs-lookup"><span data-stu-id="47f54-118">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="47f54-119">macKey</span><span class="sxs-lookup"><span data-stu-id="47f54-119">macKey</span></span>|<span data-ttu-id="47f54-120">Binária</span><span class="sxs-lookup"><span data-stu-id="47f54-120">Binary</span></span>|<span data-ttu-id="47f54-121">Chave usada para acessar mac.</span><span class="sxs-lookup"><span data-stu-id="47f54-121">The key used to get mac.</span></span>|
|<span data-ttu-id="47f54-122">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="47f54-122">profileIdentifier</span></span>|<span data-ttu-id="47f54-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="47f54-123">String</span></span>|<span data-ttu-id="47f54-124">O identificador de perfil.</span><span class="sxs-lookup"><span data-stu-id="47f54-124">The the profile identifier.</span></span>|
|<span data-ttu-id="47f54-125">fileDigest</span><span class="sxs-lookup"><span data-stu-id="47f54-125">fileDigest</span></span>|<span data-ttu-id="47f54-126">Binária</span><span class="sxs-lookup"><span data-stu-id="47f54-126">Binary</span></span>|<span data-ttu-id="47f54-127">O resumo de arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="47f54-127">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="47f54-128">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="47f54-128">fileDigestAlgorithm</span></span>|<span data-ttu-id="47f54-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="47f54-129">String</span></span>|<span data-ttu-id="47f54-130">O algoritmo de conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="47f54-130">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47f54-131">Relações</span><span class="sxs-lookup"><span data-stu-id="47f54-131">Relationships</span></span>
<span data-ttu-id="47f54-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="47f54-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="47f54-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="47f54-133">JSON Representation</span></span>
<span data-ttu-id="47f54-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="47f54-134">Here is a JSON representation of the resource.</span></span>
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



