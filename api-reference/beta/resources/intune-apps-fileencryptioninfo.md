---
title: Tipo de recurso fileEncryptionInfo
description: Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 18ff7b9d64473048b6d1d45069ab19549c83e0df
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960116"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="de5f2-103">Tipo de recurso fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="de5f2-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="de5f2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="de5f2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de5f2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="de5f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="de5f2-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="de5f2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de5f2-107">Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.</span><span class="sxs-lookup"><span data-stu-id="de5f2-107">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="de5f2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="de5f2-108">Properties</span></span>
|<span data-ttu-id="de5f2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de5f2-109">Property</span></span>|<span data-ttu-id="de5f2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="de5f2-110">Type</span></span>|<span data-ttu-id="de5f2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="de5f2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de5f2-112">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="de5f2-112">encryptionKey</span></span>|<span data-ttu-id="de5f2-113">Binária</span><span class="sxs-lookup"><span data-stu-id="de5f2-113">Binary</span></span>|<span data-ttu-id="de5f2-114">A chave usada para criptografar o conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="de5f2-114">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="de5f2-115">initializationVector</span><span class="sxs-lookup"><span data-stu-id="de5f2-115">initializationVector</span></span>|<span data-ttu-id="de5f2-116">Binária</span><span class="sxs-lookup"><span data-stu-id="de5f2-116">Binary</span></span>|<span data-ttu-id="de5f2-117">O vetor de inicialização usado para o algoritmo de criptografia.</span><span class="sxs-lookup"><span data-stu-id="de5f2-117">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="de5f2-118">mac</span><span class="sxs-lookup"><span data-stu-id="de5f2-118">mac</span></span>|<span data-ttu-id="de5f2-119">Binária</span><span class="sxs-lookup"><span data-stu-id="de5f2-119">Binary</span></span>|<span data-ttu-id="de5f2-120">O hash do conteúdo do arquivo criptografado + IV (hash conteúdo).</span><span class="sxs-lookup"><span data-stu-id="de5f2-120">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="de5f2-121">macKey</span><span class="sxs-lookup"><span data-stu-id="de5f2-121">macKey</span></span>|<span data-ttu-id="de5f2-122">Binária</span><span class="sxs-lookup"><span data-stu-id="de5f2-122">Binary</span></span>|<span data-ttu-id="de5f2-123">Chave usada para acessar mac.</span><span class="sxs-lookup"><span data-stu-id="de5f2-123">The key used to get mac.</span></span>|
|<span data-ttu-id="de5f2-124">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="de5f2-124">profileIdentifier</span></span>|<span data-ttu-id="de5f2-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de5f2-125">String</span></span>|<span data-ttu-id="de5f2-126">O identificador de perfil.</span><span class="sxs-lookup"><span data-stu-id="de5f2-126">The the profile identifier.</span></span>|
|<span data-ttu-id="de5f2-127">fileDigest</span><span class="sxs-lookup"><span data-stu-id="de5f2-127">fileDigest</span></span>|<span data-ttu-id="de5f2-128">Binária</span><span class="sxs-lookup"><span data-stu-id="de5f2-128">Binary</span></span>|<span data-ttu-id="de5f2-129">O resumo de arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="de5f2-129">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="de5f2-130">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="de5f2-130">fileDigestAlgorithm</span></span>|<span data-ttu-id="de5f2-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de5f2-131">String</span></span>|<span data-ttu-id="de5f2-132">O algoritmo de conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="de5f2-132">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de5f2-133">Relações</span><span class="sxs-lookup"><span data-stu-id="de5f2-133">Relationships</span></span>
<span data-ttu-id="de5f2-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="de5f2-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="de5f2-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="de5f2-135">JSON Representation</span></span>
<span data-ttu-id="de5f2-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="de5f2-136">Here is a JSON representation of the resource.</span></span>
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





