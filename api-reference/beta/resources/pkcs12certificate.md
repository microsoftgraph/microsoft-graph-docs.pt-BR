---
title: Tipo de recurso pkcs12Certificate
description: Representa a configuração para carregar um pkcs12Certificate em uma chamada de API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f312a7be0bd29d57c1a6b7dc5c7e5d72e6d41206
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509367"
---
# <a name="pkcs12certificate-resource-type"></a><span data-ttu-id="8912e-103">Tipo de recurso pkcs12Certificate</span><span class="sxs-lookup"><span data-stu-id="8912e-103">pkcs12Certificate resource type</span></span>

<span data-ttu-id="8912e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8912e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8912e-105">Representa a configuração usada para **carregar um** certificado ao usar a autenticação de certificado de cliente HTTPS para chamar um ponto de extremidade do conector de API.</span><span class="sxs-lookup"><span data-stu-id="8912e-105">Represents the configuration used to **upload** a certificate when using HTTPS client-certificate authentication for calling an API connector endpoint.</span></span> <span data-ttu-id="8912e-106">A autenticação de certificado de cliente é uma autenticação mútua baseada em certificado, onde o cliente fornece um certificado de cliente para um ponto de extremidade da API para comprovar sua identidade.</span><span class="sxs-lookup"><span data-stu-id="8912e-106">Client certificate authentication is a mutual certificate-based authentication, where the client provides a client certificate to an API endpoint to prove its identity.</span></span> <span data-ttu-id="8912e-107">O certificado configurado de um conector de API é enviado pelo Azure AD para o ponto de extremidade da API determinado, que valida o certificado.</span><span class="sxs-lookup"><span data-stu-id="8912e-107">The configured certificate of an API connector is sent by Azure AD to the given API endpoint, which then validates the certificate.</span></span>

<span data-ttu-id="8912e-108">Herda de [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="8912e-108">Inherits from [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8912e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8912e-109">Properties</span></span>

|<span data-ttu-id="8912e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8912e-110">Property</span></span>|<span data-ttu-id="8912e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="8912e-111">Type</span></span>|<span data-ttu-id="8912e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="8912e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8912e-113">pkcs12Value</span><span class="sxs-lookup"><span data-stu-id="8912e-113">pkcs12Value</span></span>|<span data-ttu-id="8912e-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8912e-114">String</span></span>| <span data-ttu-id="8912e-115">Este é o campo para o envio de conteúdo pfx.</span><span class="sxs-lookup"><span data-stu-id="8912e-115">This is the field for sending pfx content.</span></span> <span data-ttu-id="8912e-116">O valor deve ser uma versão codificada de base 64 do conteúdo real do certificado.</span><span class="sxs-lookup"><span data-stu-id="8912e-116">The value should be a base-64 encoded version of the actual certificate content.</span></span> <span data-ttu-id="8912e-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8912e-117">Required.</span></span>|
|<span data-ttu-id="8912e-118">password</span><span class="sxs-lookup"><span data-stu-id="8912e-118">password</span></span>|<span data-ttu-id="8912e-119">String</span><span class="sxs-lookup"><span data-stu-id="8912e-119">String</span></span>| <span data-ttu-id="8912e-120">Essa é a senha do arquivo pfx.</span><span class="sxs-lookup"><span data-stu-id="8912e-120">This is the password for the pfx file.</span></span> <span data-ttu-id="8912e-121">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8912e-121">Required.</span></span> <span data-ttu-id="8912e-122">Se nenhuma senha for usada, ainda deverá fornecer um valor `""` de .</span><span class="sxs-lookup"><span data-stu-id="8912e-122">If no password is used, must still provide a value of `""`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8912e-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8912e-123">JSON representation</span></span>

<span data-ttu-id="8912e-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8912e-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.pkcs12Certificate"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.pkcs12Certificate",
  "pkcs12Value": "String",
  "password": "String"
}
```
