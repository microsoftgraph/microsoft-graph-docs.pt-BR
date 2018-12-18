---
title: ação de createGooglePlayWebToken
description: Gera um token de web que é usado em um componente incorporável.
author: tfitzmac
ms.openlocfilehash: 206113b445d8b190e02b292dd661bc3c207de288
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338539"
---
# <a name="creategoogleplaywebtoken-action"></a><span data-ttu-id="f8053-103">ação de createGooglePlayWebToken</span><span class="sxs-lookup"><span data-stu-id="f8053-103">createGooglePlayWebToken action</span></span>

> <span data-ttu-id="f8053-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f8053-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8053-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f8053-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8053-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f8053-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8053-107">Gera um token de web que é usado em um componente incorporável.</span><span class="sxs-lookup"><span data-stu-id="f8053-107">Generates a web token that is used in an embeddable component.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f8053-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f8053-108">Prerequisites</span></span>
<span data-ttu-id="f8053-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8053-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8053-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8053-111">Permission type</span></span>|<span data-ttu-id="f8053-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f8053-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8053-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8053-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8053-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8053-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f8053-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8053-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8053-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8053-116">Not supported.</span></span>|
|<span data-ttu-id="f8053-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8053-117">Application</span></span>|<span data-ttu-id="f8053-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8053-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8053-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8053-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken
```

## <a name="request-headers"></a><span data-ttu-id="f8053-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8053-120">Request headers</span></span>
|<span data-ttu-id="f8053-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f8053-121">Header</span></span>|<span data-ttu-id="f8053-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f8053-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8053-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8053-123">Authorization</span></span>|<span data-ttu-id="f8053-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8053-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8053-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f8053-125">Accept</span></span>|<span data-ttu-id="f8053-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8053-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8053-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8053-127">Request body</span></span>
<span data-ttu-id="f8053-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f8053-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f8053-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="f8053-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f8053-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8053-130">Property</span></span>|<span data-ttu-id="f8053-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8053-131">Type</span></span>|<span data-ttu-id="f8053-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8053-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8053-133">parentUri</span><span class="sxs-lookup"><span data-stu-id="f8053-133">parentUri</span></span>|<span data-ttu-id="f8053-134">String</span><span class="sxs-lookup"><span data-stu-id="f8053-134">String</span></span>|<span data-ttu-id="f8053-135">O caminho de https da página que hospeda o componente.</span><span class="sxs-lookup"><span data-stu-id="f8053-135">The https path of the page hosting the component.</span></span>|



## <a name="response"></a><span data-ttu-id="f8053-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8053-136">Response</span></span>
<span data-ttu-id="f8053-137">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e uma cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8053-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8053-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8053-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="f8053-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8053-139">Request</span></span>
<span data-ttu-id="f8053-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8053-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken

Content-type: application/json
Content-length: 39

{
  "parentUri": "Parent Uri value"
}
```

### <a name="response"></a><span data-ttu-id="f8053-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8053-141">Response</span></span>
<span data-ttu-id="f8053-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8053-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 53

{
  "value": "Create Google Play Web Token value"
}
```





