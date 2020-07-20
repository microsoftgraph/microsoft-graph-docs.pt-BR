---
title: 'impressora: criar'
description: Cria (registra) uma impressora com o serviço de impressão universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a0b64166b6d7c95f3ad4995321b50b2c4aaadda9
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081058"
---
# <a name="printer-create"></a><span data-ttu-id="08d11-103">impressora: criar</span><span class="sxs-lookup"><span data-stu-id="08d11-103">printer: create</span></span>

<span data-ttu-id="08d11-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08d11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08d11-105">Criar (registrar) uma impressora com o serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="08d11-105">Create (register) a printer with the Universal Print service.</span></span> <span data-ttu-id="08d11-106">Esta é uma operação de execução demorada e, como tal, retorna um [printerCreateOperation](../resources/printercreateoperation.md) que pode ser usado para rastrear e verificar o registro da impressora.</span><span class="sxs-lookup"><span data-stu-id="08d11-106">This is a long-running operation and as such, it returns a [printerCreateOperation](../resources/printercreateoperation.md) that can be used to track and verify the registration of the printer.</span></span>

## <a name="permissions"></a><span data-ttu-id="08d11-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="08d11-107">Permissions</span></span>
<span data-ttu-id="08d11-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08d11-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="08d11-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="08d11-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="08d11-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08d11-111">Permission type</span></span> | <span data-ttu-id="08d11-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="08d11-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="08d11-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08d11-113">Delegated (work or school account)</span></span>| <span data-ttu-id="08d11-114">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="08d11-114">User.Read.All</span></span> |
|<span data-ttu-id="08d11-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08d11-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08d11-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08d11-116">Not Supported.</span></span>|
|<span data-ttu-id="08d11-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08d11-117">Application</span></span>|<span data-ttu-id="08d11-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08d11-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08d11-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08d11-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/create
```
## <a name="request-headers"></a><span data-ttu-id="08d11-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08d11-120">Request headers</span></span>
| <span data-ttu-id="08d11-121">Nome</span><span class="sxs-lookup"><span data-stu-id="08d11-121">Name</span></span>       | <span data-ttu-id="08d11-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="08d11-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="08d11-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="08d11-123">Authorization</span></span> | <span data-ttu-id="08d11-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08d11-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="08d11-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="08d11-126">Content-type</span></span>  | <span data-ttu-id="08d11-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08d11-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="08d11-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08d11-129">Request body</span></span>
<span data-ttu-id="08d11-130">No corpo da solicitação, forneça um objeto JSON com as propriedades a seguir.</span><span class="sxs-lookup"><span data-stu-id="08d11-130">In the request body, provide a JSON object with the following properties.</span></span>

| <span data-ttu-id="08d11-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="08d11-131">Parameter</span></span>      | <span data-ttu-id="08d11-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="08d11-132">Type</span></span>    |<span data-ttu-id="08d11-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="08d11-133">Description</span></span>| <span data-ttu-id="08d11-134">Obrigatório?</span><span class="sxs-lookup"><span data-stu-id="08d11-134">Required?</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="08d11-135">displayName</span><span class="sxs-lookup"><span data-stu-id="08d11-135">displayName</span></span>|<span data-ttu-id="08d11-136">String</span><span class="sxs-lookup"><span data-stu-id="08d11-136">String</span></span>|<span data-ttu-id="08d11-137">O nome de exibição a ser atribuído à impressora.</span><span class="sxs-lookup"><span data-stu-id="08d11-137">The display name to assign to the printer.</span></span>|<span data-ttu-id="08d11-138">Sim</span><span class="sxs-lookup"><span data-stu-id="08d11-138">Yes</span></span>|
|<span data-ttu-id="08d11-139">fabricante</span><span class="sxs-lookup"><span data-stu-id="08d11-139">manufacturer</span></span>|<span data-ttu-id="08d11-140">String</span><span class="sxs-lookup"><span data-stu-id="08d11-140">String</span></span>|<span data-ttu-id="08d11-141">O fabricante da impressora.</span><span class="sxs-lookup"><span data-stu-id="08d11-141">The manufacturer of the printer.</span></span>|<span data-ttu-id="08d11-142">Sim</span><span class="sxs-lookup"><span data-stu-id="08d11-142">Yes</span></span>|
|<span data-ttu-id="08d11-143">modelo</span><span class="sxs-lookup"><span data-stu-id="08d11-143">model</span></span>|<span data-ttu-id="08d11-144">String</span><span class="sxs-lookup"><span data-stu-id="08d11-144">String</span></span>|<span data-ttu-id="08d11-145">O modelo da impressora.</span><span class="sxs-lookup"><span data-stu-id="08d11-145">The model of the printer.</span></span>|<span data-ttu-id="08d11-146">Sim</span><span class="sxs-lookup"><span data-stu-id="08d11-146">Yes</span></span>|
|<span data-ttu-id="08d11-147">physicalDeviceId</span><span class="sxs-lookup"><span data-stu-id="08d11-147">physicalDeviceId</span></span>|<span data-ttu-id="08d11-148">String</span><span class="sxs-lookup"><span data-stu-id="08d11-148">String</span></span>|<span data-ttu-id="08d11-149">O UUID do dispositivo físico da impressora.</span><span class="sxs-lookup"><span data-stu-id="08d11-149">The physical device UUID of the printer.</span></span> <span data-ttu-id="08d11-150">Obrigatório se a `hasPhysicalDevice` propriedade for true.</span><span class="sxs-lookup"><span data-stu-id="08d11-150">Required if the `hasPhysicalDevice` property is true.</span></span>|<span data-ttu-id="08d11-151">Não</span><span class="sxs-lookup"><span data-stu-id="08d11-151">No</span></span>|
|<span data-ttu-id="08d11-152">hasPhysicalDevice</span><span class="sxs-lookup"><span data-stu-id="08d11-152">hasPhysicalDevice</span></span>|<span data-ttu-id="08d11-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="08d11-153">Boolean</span></span>|<span data-ttu-id="08d11-154">True se a impressora tem dispositivo de saída físico; caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="08d11-154">True if the printer has physical output device, false otherwise.</span></span> <span data-ttu-id="08d11-155">Se for omitido, o valor padrão será true.</span><span class="sxs-lookup"><span data-stu-id="08d11-155">If omitted, the default value is true.</span></span>|<span data-ttu-id="08d11-156">Não</span><span class="sxs-lookup"><span data-stu-id="08d11-156">No</span></span>|
|<span data-ttu-id="08d11-157">certificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="08d11-157">certificateSigningRequest</span></span>|[<span data-ttu-id="08d11-158">printCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="08d11-158">printCertificateSigningRequest</span></span>](../resources/printcertificatesigningrequest.md)|<span data-ttu-id="08d11-159">A solicitação de assinatura de certificado (CSR) do X. 509 para o certificado criado e usado pela impressora para identificar-se.</span><span class="sxs-lookup"><span data-stu-id="08d11-159">The X.509 Certificate Signing Request (CSR) for the certificate created and used by the printer to identify itself.</span></span>|<span data-ttu-id="08d11-160">Sim</span><span class="sxs-lookup"><span data-stu-id="08d11-160">Yes</span></span>|
|<span data-ttu-id="08d11-161">connectorid</span><span class="sxs-lookup"><span data-stu-id="08d11-161">connectorId</span></span>|<span data-ttu-id="08d11-162">String</span><span class="sxs-lookup"><span data-stu-id="08d11-162">String</span></span>|<span data-ttu-id="08d11-163">ID do conector que atua como proxy para a impressora.</span><span class="sxs-lookup"><span data-stu-id="08d11-163">Id of Connector acting as proxy to the printer.</span></span>|<span data-ttu-id="08d11-164">Não</span><span class="sxs-lookup"><span data-stu-id="08d11-164">No</span></span>|

## <a name="response"></a><span data-ttu-id="08d11-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="08d11-165">Response</span></span>
<span data-ttu-id="08d11-166">Se tiver êxito, este método retornará um `202 Accepted` código de resposta e um link para o [printerCreateOperation](../resources/printercreateoperation.md) associado no `Operation-Location` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="08d11-166">If successful, this method returns a `202 Accepted` response code and a link to the associated [printerCreateOperation](../resources/printercreateoperation.md) in the `Operation-Location` header.</span></span>

<span data-ttu-id="08d11-167">Fazer uma solicitação GET para a URL vinculada pode ser usado para obter o status de um registro de impressora em andamento.</span><span class="sxs-lookup"><span data-stu-id="08d11-167">Making a GET request to the linked URL can be used to get the status of an ongoing printer registration.</span></span> <span data-ttu-id="08d11-168">Após o registro da impressora ter sido concluído com êxito, uma solicitação GET para a URL vinculada conterá o objeto Printer criado e o certificado registrado.</span><span class="sxs-lookup"><span data-stu-id="08d11-168">Once printer registration has completed successfully, a GET request to the linked URL will contain the created printer object and registered certificate.</span></span>

## <a name="example"></a><span data-ttu-id="08d11-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08d11-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="08d11-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08d11-170">Request</span></span>
<span data-ttu-id="08d11-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="08d11-171">The following is an example of the request.</span></span> <span data-ttu-id="08d11-172">Para obter ajuda para criar a solicitação de assinatura de certificado (CSR) necessária, consulte o [exemplo de código de geração de CSR](https://docs.microsoft.com/universal-print/hardware/universal-print-oem-certificate-signing-request).</span><span class="sxs-lookup"><span data-stu-id="08d11-172">For help creating the required Certificate Signing Request (CSR), see the [CSR generation code sample](https://docs.microsoft.com/universal-print/hardware/universal-print-oem-certificate-signing-request).</span></span>


# <a name="http"></a>[<span data-ttu-id="08d11-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="08d11-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printer"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/create
Content-type: application/json
Content-length: 319

{
  "displayName": "Test Printer",
  "manufacturer": "Test Printer Manufacturer",
  "model": "Test Printer Model",
  "physicalDeviceId": null,
  "hasPhysicalDevice": false,
  "certificateSigningRequest": { 
    "content": "{content}",
    "transportKey": "{sampleTransportKey}"
  },
  "connectorId": null
}
```
# <a name="javascript"></a>[<span data-ttu-id="08d11-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08d11-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="08d11-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="08d11-175">Response</span></span>
<span data-ttu-id="08d11-176">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="08d11-176">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
Operation-Location: https://graph.microsoft.com/beta/print/operations/f221760a-52e8-4c11-b8c5-5dfaef3a49db
Retry-After: 5
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printers: create",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
