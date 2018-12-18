---
title: Tipo de recurso fileEncryptionInfo
description: Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.
author: tfitzmac
ms.openlocfilehash: a13c451193d248d09e020cc6b308b9f03d991295
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307850"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="dd4bb-103">Tipo de recurso fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="dd4bb-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="dd4bb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dd4bb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd4bb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dd4bb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dd4bb-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="dd4bb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd4bb-107">Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.</span><span class="sxs-lookup"><span data-stu-id="dd4bb-107">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="dd4bb-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dd4bb-108">Properties</span></span>
|<span data-ttu-id="dd4bb-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd4bb-109">Property</span></span>|<span data-ttu-id="dd4bb-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd4bb-110">Type</span></span>|<span data-ttu-id="dd4bb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd4bb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd4bb-112">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="dd4bb-112">encryptionKey</span></span>|<span data-ttu-id="dd4bb-113">Binária</span><span class="sxs-lookup"><span data-stu-id="dd4bb-113">Binary</span></span>|<span data-ttu-id="dd4bb-114">A chave usada para criptografar o conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="dd4bb-114">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="dd4bb-115">initializationVector</span><span class="sxs-lookup"><span data-stu-id="dd4bb-115">initializationVector</span></span>|<span data-ttu-id="dd4bb-116">Binária</span><span class="sxs-lookup"><span data-stu-id="dd4bb-116">Binary</span></span>|<span data-ttu-id="dd4bb-117">O vetor de inicialização usado para o algoritmo de criptografia.</span><span class="sxs-lookup"><span data-stu-id="dd4bb-117">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="dd4bb-118">mac</span><span class="sxs-lookup"><span data-stu-id="dd4bb-118">mac</span></span>|<span data-ttu-id="dd4bb-119">Binária</span><span class="sxs-lookup"><span data-stu-id="dd4bb-119">Binary</span></span>|<span data-ttu-id="dd4bb-120">O hash do conteúdo do arquivo criptografado + IV (hash conteúdo).</span><span class="sxs-lookup"><span data-stu-id="dd4bb-120">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="dd4bb-121">macKey</span><span class="sxs-lookup"><span data-stu-id="dd4bb-121">macKey</span></span>|<span data-ttu-id="dd4bb-122">Binária</span><span class="sxs-lookup"><span data-stu-id="dd4bb-122">Binary</span></span>|<span data-ttu-id="dd4bb-123">Chave usada para acessar mac.</span><span class="sxs-lookup"><span data-stu-id="dd4bb-123">The key used to get mac.</span></span>|
|<span data-ttu-id="dd4bb-124">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="dd4bb-124">profileIdentifier</span></span>|<span data-ttu-id="dd4bb-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd4bb-125">String</span></span>|<span data-ttu-id="dd4bb-126">O identificador de perfil.</span><span class="sxs-lookup"><span data-stu-id="dd4bb-126">The the profile identifier.</span></span>|
|<span data-ttu-id="dd4bb-127">fileDigest</span><span class="sxs-lookup"><span data-stu-id="dd4bb-127">fileDigest</span></span>|<span data-ttu-id="dd4bb-128">Binária</span><span class="sxs-lookup"><span data-stu-id="dd4bb-128">Binary</span></span>|<span data-ttu-id="dd4bb-129">O resumo de arquivo antes da criptografia.</span><span class="sxs-lookup"><span data-stu-id="dd4bb-129">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="dd4bb-130">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="dd4bb-130">fileDigestAlgorithm</span></span>|<span data-ttu-id="dd4bb-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd4bb-131">String</span></span>|<span data-ttu-id="dd4bb-132">O algoritmo de conteúdo do arquivo.</span><span class="sxs-lookup"><span data-stu-id="dd4bb-132">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd4bb-133">Relações</span><span class="sxs-lookup"><span data-stu-id="dd4bb-133">Relationships</span></span>
<span data-ttu-id="dd4bb-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dd4bb-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dd4bb-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dd4bb-135">JSON Representation</span></span>
<span data-ttu-id="dd4bb-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dd4bb-136">Here is a JSON representation of the resource.</span></span>
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





