---
title: ação createGooglePlayWebToken
description: Gera um token da Web que é usado em um componente inbeddável.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6cc813873b865eb03c76a68f40141b3b42bac044
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141194"
---
# <a name="creategoogleplaywebtoken-action"></a><span data-ttu-id="be52a-103">ação createGooglePlayWebToken</span><span class="sxs-lookup"><span data-stu-id="be52a-103">createGooglePlayWebToken action</span></span>

<span data-ttu-id="be52a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be52a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="be52a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="be52a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be52a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="be52a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be52a-107">Gera um token da Web que é usado em um componente inbeddável.</span><span class="sxs-lookup"><span data-stu-id="be52a-107">Generates a web token that is used in an embeddable component.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be52a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="be52a-108">Prerequisites</span></span>
<span data-ttu-id="be52a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be52a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be52a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be52a-111">Permission type</span></span>|<span data-ttu-id="be52a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="be52a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be52a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be52a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="be52a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be52a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="be52a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be52a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be52a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be52a-116">Not supported.</span></span>|
|<span data-ttu-id="be52a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be52a-117">Application</span></span>|<span data-ttu-id="be52a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be52a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="be52a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be52a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken
```

## <a name="request-headers"></a><span data-ttu-id="be52a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be52a-120">Request headers</span></span>
|<span data-ttu-id="be52a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="be52a-121">Header</span></span>|<span data-ttu-id="be52a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="be52a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be52a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="be52a-123">Authorization</span></span>|<span data-ttu-id="be52a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be52a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be52a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="be52a-125">Accept</span></span>|<span data-ttu-id="be52a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="be52a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be52a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be52a-127">Request body</span></span>
<span data-ttu-id="be52a-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="be52a-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="be52a-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="be52a-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="be52a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be52a-130">Property</span></span>|<span data-ttu-id="be52a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="be52a-131">Type</span></span>|<span data-ttu-id="be52a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="be52a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be52a-133">parentUri</span><span class="sxs-lookup"><span data-stu-id="be52a-133">parentUri</span></span>|<span data-ttu-id="be52a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="be52a-134">String</span></span>|<span data-ttu-id="be52a-135">O caminho https da página que hospeda o componente.</span><span class="sxs-lookup"><span data-stu-id="be52a-135">The https path of the page hosting the component.</span></span>|



## <a name="response"></a><span data-ttu-id="be52a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="be52a-136">Response</span></span>
<span data-ttu-id="be52a-137">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e uma cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be52a-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be52a-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="be52a-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="be52a-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be52a-139">Request</span></span>
<span data-ttu-id="be52a-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="be52a-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken

Content-type: application/json
Content-length: 39

{
  "parentUri": "Parent Uri value"
}
```

### <a name="response"></a><span data-ttu-id="be52a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="be52a-141">Response</span></span>
<span data-ttu-id="be52a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="be52a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 53

{
  "value": "Create Google Play Web Token value"
}
```




