---
title: Tipo de recurso fileEncryptionInfo
description: Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 074bf24638bf0ba7d613399e1b8894de7f30dfbb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410893"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="e2534-103">Tipo de recurso fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="e2534-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="e2534-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="e2534-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e2534-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e2534-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2534-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="e2534-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2534-107">Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.</span><span class="sxs-lookup"><span data-stu-id="e2534-107">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="e2534-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2534-108">Properties</span></span>
|<span data-ttu-id="e2534-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2534-109">Property</span></span>|<span data-ttu-id="e2534-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2534-110">Type</span></span>|<span data-ttu-id="e2534-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2534-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2534-112">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="e2534-112">encryptionKey</span></span>|<span data-ttu-id="e2534-113">Binária</span><span class="sxs-lookup"><span data-stu-id="e2534-113">Binary</span></span>|<span data-ttu-id="e2534-114">A chave usada para criptografar o conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="e2534-114">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="e2534-115">initializationVector</span><span class="sxs-lookup"><span data-stu-id="e2534-115">initializationVector</span></span>|<span data-ttu-id="e2534-116">Binária</span><span class="sxs-lookup"><span data-stu-id="e2534-116">Binary</span></span>|<span data-ttu-id="e2534-117">O vetor de inicialização usado para o algoritmo de criptografia.</span><span class="sxs-lookup"><span data-stu-id="e2534-117">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="e2534-118">mac</span><span class="sxs-lookup"><span data-stu-id="e2534-118">mac</span></span>|<span data-ttu-id="e2534-119">Binária</span><span class="sxs-lookup"><span data-stu-id="e2534-119">Binary</span></span>|<span data-ttu-id="e2534-120">O hash do conteúdo do arquivo criptografado + IV (hash conteúdo).</span><span class="sxs-lookup"><span data-stu-id="e2534-120">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="e2534-121">macKey</span><span class="sxs-lookup"><span data-stu-id="e2534-121">macKey</span></span>|<span data-ttu-id="e2534-122">Binária</span><span class="sxs-lookup"><span data-stu-id="e2534-122">Binary</span></span>|<span data-ttu-id="e2534-123">Chave usada para acessar mac.</span><span class="sxs-lookup"><span data-stu-id="e2534-123">The key used to get mac.</span></span>|
|<span data-ttu-id="e2534-124">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="e2534-124">profileIdentifier</span></span>|<span data-ttu-id="e2534-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2534-125">String</span></span>|<span data-ttu-id="e2534-126">O identificador de perfil.</span><span class="sxs-lookup"><span data-stu-id="e2534-126">The the profile identifier.</span></span>|
|<span data-ttu-id="e2534-127">fileDigest</span><span class="sxs-lookup"><span data-stu-id="e2534-127">fileDigest</span></span>|<span data-ttu-id="e2534-128">Binária</span><span class="sxs-lookup"><span data-stu-id="e2534-128">Binary</span></span>|<span data-ttu-id="e2534-129">O resumo de arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="e2534-129">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="e2534-130">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="e2534-130">fileDigestAlgorithm</span></span>|<span data-ttu-id="e2534-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2534-131">String</span></span>|<span data-ttu-id="e2534-132">O algoritmo de conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="e2534-132">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2534-133">Relações</span><span class="sxs-lookup"><span data-stu-id="e2534-133">Relationships</span></span>
<span data-ttu-id="e2534-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e2534-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2534-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2534-135">JSON Representation</span></span>
<span data-ttu-id="e2534-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e2534-136">Here is a JSON representation of the resource.</span></span>
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




