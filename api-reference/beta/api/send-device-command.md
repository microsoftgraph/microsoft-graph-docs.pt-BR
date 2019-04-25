---
title: Enviar comando do dispositivo
description: 'Essa API permite que os recursos do Project Roma para o comando um dispositivo associado a uma conta da Microsoft. Depois de obter uma chamada GET `me/devices`, passe a ID do dispositivo para emitir um comando para seu dispositivo. Há suporte para dois tipos de comandos: LaunchURI e AppServices. Se você estiver usando o LaunchURI, especifique os parâmetros *Type* e *Payload* . Para uma chamada serviço, especifique o '
localization_priority: Normal
ms.openlocfilehash: d0c25200933a4a87a66349e457c500c496272b08
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537522"
---
# <a name="send-device-command"></a><span data-ttu-id="f1aa3-107">Enviar comando do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f1aa3-107">Send device command</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1aa3-108">Essa API permite que os recursos do Project Roma para o comando um dispositivo associado a uma conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f1aa3-108">This API enables Project Rome capabilities to command a device associated with a Microsoft account.</span></span> <span data-ttu-id="f1aa3-109">Depois de obter uma chamada GET `me/devices`, passe a ID do dispositivo para emitir um comando para seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f1aa3-109">After doing a GET call on `me/devices`, pass in the ID of the device to issue a command to your device.</span></span> <span data-ttu-id="f1aa3-110">Há suporte para dois tipos de comandos: LaunchURI e AppServices.</span><span class="sxs-lookup"><span data-stu-id="f1aa3-110">Two types of commands are supported: LaunchURI and AppServices.</span></span> <span data-ttu-id="f1aa3-111">Se você estiver usando o LaunchURI, especifique os parâmetros *Type* e *Payload* .</span><span class="sxs-lookup"><span data-stu-id="f1aa3-111">If you're using LaunchURI, specify the *type* and *payload* parameters.</span></span> <span data-ttu-id="f1aa3-112">Para uma chamada serviço, especifique os parâmetros *Type*, *Payload*, *packageFamilyName*e *appServiceName* .</span><span class="sxs-lookup"><span data-stu-id="f1aa3-112">For an AppService call, specify the *type*, *payload*, *packageFamilyName*, and *appServiceName* parameters.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1aa3-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1aa3-113">Permissions</span></span>

<span data-ttu-id="f1aa3-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1aa3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f1aa3-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1aa3-116">Permission type</span></span>      | <span data-ttu-id="f1aa3-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1aa3-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1aa3-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1aa3-118">Delegated (work or school account)</span></span> | <span data-ttu-id="f1aa3-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1aa3-119">Not supported.</span></span>    |
|<span data-ttu-id="f1aa3-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1aa3-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1aa3-121">Device.Command</span><span class="sxs-lookup"><span data-stu-id="f1aa3-121">Device.Command</span></span>    |
|<span data-ttu-id="f1aa3-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1aa3-122">Application</span></span> | <span data-ttu-id="f1aa3-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1aa3-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1aa3-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1aa3-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST me/devices/{id}/commands
```

## <a name="request-headers"></a><span data-ttu-id="f1aa3-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1aa3-125">Request headers</span></span>


| <span data-ttu-id="f1aa3-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1aa3-126">Header</span></span> |<span data-ttu-id="f1aa3-127">Valor</span><span class="sxs-lookup"><span data-stu-id="f1aa3-127">Value</span></span>
|:----|:------|
|<span data-ttu-id="f1aa3-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1aa3-128">Authorization</span></span>| <span data-ttu-id="f1aa3-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1aa3-p104">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="f1aa3-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f1aa3-131">Accept</span></span> | <span data-ttu-id="f1aa3-132">application/json</span><span class="sxs-lookup"><span data-stu-id="f1aa3-132">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1aa3-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1aa3-133">Request body</span></span>

<span data-ttu-id="f1aa3-134">No corpo da solicitação, forneça uma representação JSON das propriedades do comando.</span><span class="sxs-lookup"><span data-stu-id="f1aa3-134">In the request body, supply a JSON representation of the command properties.</span></span>

```json
{
  "type": "appService",
  "payload": "payload-JSON",
  "packageFamilyName": "packageFamilyName",
  "appServiceName": "appServiceName",
  "postbackURI": "postbackURI"
}
```

## <a name="response"></a><span data-ttu-id="f1aa3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1aa3-135">Response</span></span>

```http
HTTP/1.1 201 OK
```

```json
{
  "id": "0",
  "status": "requesting",
  "type": "appService",
  "appServiceName": "appServiceName",
  "packageFamilyName": "packageFamilyName",
  "error": "null",
  "responsePayload": "null",
  "payload": "payload-JSON",
  "permissionTicket": "null",
  "postBackUri": "postbackURI"
}
```
## <a name="command-properties"></a><span data-ttu-id="f1aa3-136">Propriedades de comando</span><span class="sxs-lookup"><span data-stu-id="f1aa3-136">Command properties</span></span> 

|<span data-ttu-id="f1aa3-137">**Nome**</span><span class="sxs-lookup"><span data-stu-id="f1aa3-137">**Name**</span></span>|<span data-ttu-id="f1aa3-138">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="f1aa3-138">**Type**</span></span>|<span data-ttu-id="f1aa3-139">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f1aa3-139">**Description**</span></span>|
|:----|:------|:------|
|<span data-ttu-id="f1aa3-140">payload</span><span class="sxs-lookup"><span data-stu-id="f1aa3-140">payload</span></span> | <span data-ttu-id="f1aa3-141">Microsoft. Graph. JSON</span><span class="sxs-lookup"><span data-stu-id="f1aa3-141">microsoft.graph.json</span></span>| <span data-ttu-id="f1aa3-142">Carga a ser enviada a um serviço de aplicativo ou para iniciar um URI em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f1aa3-142">Payload to send to an app service or to launch a URI on a device.</span></span> |
|<span data-ttu-id="f1aa3-143">responsePayload</span><span class="sxs-lookup"><span data-stu-id="f1aa3-143">responsePayload</span></span> | <span data-ttu-id="f1aa3-144">Microsoft. Graph. JSON</span><span class="sxs-lookup"><span data-stu-id="f1aa3-144">microsoft.graph.json</span></span>| <span data-ttu-id="f1aa3-145">Carga retornada do dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="f1aa3-145">Payload returned from target device.</span></span> |
|<span data-ttu-id="f1aa3-146">postBackURI</span><span class="sxs-lookup"><span data-stu-id="f1aa3-146">postBackURI</span></span> | <span data-ttu-id="f1aa3-147">String</span><span class="sxs-lookup"><span data-stu-id="f1aa3-147">String</span></span> | <span data-ttu-id="f1aa3-148">Postar URI para enviar notificações de atualizações subsequentes.</span><span class="sxs-lookup"><span data-stu-id="f1aa3-148">Post back URI to send subsequent notifications of updates.</span></span> |
|<span data-ttu-id="f1aa3-149">packageFamilyName</span><span class="sxs-lookup"><span data-stu-id="f1aa3-149">packageFamilyName</span></span> | <span data-ttu-id="f1aa3-150">String</span><span class="sxs-lookup"><span data-stu-id="f1aa3-150">String</span></span> | <span data-ttu-id="f1aa3-151">Nome do aplicativo da família de pacote do Windows.</span><span class="sxs-lookup"><span data-stu-id="f1aa3-151">Windows Package Family Name of application.</span></span> |
|<span data-ttu-id="f1aa3-152">appServiceName</span><span class="sxs-lookup"><span data-stu-id="f1aa3-152">appServiceName</span></span> | <span data-ttu-id="f1aa3-153">String</span><span class="sxs-lookup"><span data-stu-id="f1aa3-153">String</span></span> | <span data-ttu-id="f1aa3-154">Nome do serviço de aplicativo definido pelo aplicativo de destino.</span><span class="sxs-lookup"><span data-stu-id="f1aa3-154">Name of app service defined by the target application.</span></span> <span data-ttu-id="f1aa3-155">Necessário se iniciar um serviço de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f1aa3-155">Required if launching an app service.</span></span> |
|<span data-ttu-id="f1aa3-156">type</span><span class="sxs-lookup"><span data-stu-id="f1aa3-156">type</span></span>| <span data-ttu-id="f1aa3-157">String</span><span class="sxs-lookup"><span data-stu-id="f1aa3-157">String</span></span> | <span data-ttu-id="f1aa3-158">LaunchURI ou serviço.</span><span class="sxs-lookup"><span data-stu-id="f1aa3-158">LaunchURI or AppService.</span></span> |
|<span data-ttu-id="f1aa3-159">id</span><span class="sxs-lookup"><span data-stu-id="f1aa3-159">id</span></span>| <span data-ttu-id="f1aa3-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1aa3-160">String</span></span> | <span data-ttu-id="f1aa3-161">A ID de um comando que foi enviado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f1aa3-161">The ID of a command that has been sent to the device.</span></span> |
|<span data-ttu-id="f1aa3-162">actionStatus</span><span class="sxs-lookup"><span data-stu-id="f1aa3-162">actionStatus</span></span> | <span data-ttu-id="f1aa3-163">String</span><span class="sxs-lookup"><span data-stu-id="f1aa3-163">String</span></span> | <span data-ttu-id="f1aa3-164">O [status](get-device-command-status.md) de um comando.</span><span class="sxs-lookup"><span data-stu-id="f1aa3-164">The [status](get-device-command-status.md) of a command.</span></span> |
|<span data-ttu-id="f1aa3-165">erro</span><span class="sxs-lookup"><span data-stu-id="f1aa3-165">error</span></span>| <span data-ttu-id="f1aa3-166">String</span><span class="sxs-lookup"><span data-stu-id="f1aa3-166">String</span></span>| <span data-ttu-id="f1aa3-167">Quaisquer erros associados à solicitação do aplicativo de destino.</span><span class="sxs-lookup"><span data-stu-id="f1aa3-167">Any errors associated with the request from the target application.</span></span> |

## <a name="launch-uri-example"></a><span data-ttu-id="f1aa3-168">Exemplo de URI de inicialização</span><span class="sxs-lookup"><span data-stu-id="f1aa3-168">Launch URI example</span></span>

<span data-ttu-id="f1aa3-169">Aqui está um exemplo de uma solicitação LaunchURI; ele iniciará um URI ou um aplicativo no dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="f1aa3-169">Here is an example of a LaunchURI request; it will launch a URI or an application on the target device.</span></span> <span data-ttu-id="f1aa3-170">Para iniciar um URI ou um aplicativo, emita uma POSTAgem usando a ID do dispositivo (obtido de uma chamada GET ativada `me/devices`).</span><span class="sxs-lookup"><span data-stu-id="f1aa3-170">To launch a URI or an app, issue a POST using the ID of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="f1aa3-171">Defina os parâmetros de *tipo* como *LaunchURI* e forneça um valor de URI https://bing.comcomo.</span><span class="sxs-lookup"><span data-stu-id="f1aa3-171">Set the *Type* parameters to *LaunchURI* and provide a URI value such as https://bing.com.</span></span>

#### <a name="request"></a><span data-ttu-id="f1aa3-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1aa3-172">Request</span></span>

<span data-ttu-id="f1aa3-173">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1aa3-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_command"
} -->

```http

POST me/devices/{id}/commands
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8

{ "type" : "LaunchUri", "payload" : {"uri":"https://bing.com"}}

```

#### <a name="response"></a><span data-ttu-id="f1aa3-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1aa3-174">Response</span></span> 

<span data-ttu-id="f1aa3-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f1aa3-175">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
  "isCollection": true
} -->

```http
HTTP/1.1 201 OK

{
  "id": "0158355AD4D680CC4E2994CC009EFFD7337D1B...",
  "status": "requesting",
  "type": null,
  "appServiceName": null,
  "packageFamilyName": null,
  "error": null,
  "permissionTicket": null,
  "postBackUri": null,
  "payload": {
    "uri": "https://bing.com"
  }
}

```


## <a name="app-service-example"></a><span data-ttu-id="f1aa3-176">Exemplo de serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1aa3-176">App service example</span></span>

<span data-ttu-id="f1aa3-177">Veja um exemplo de consulta de um serviço de aplicativo em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f1aa3-177">Here is an example of querying an app service on a device.</span></span> <span data-ttu-id="f1aa3-178">Para usar um serviço de aplicativo, você deve fazer uma chamada POST usando a ID do dispositivo (obtido de uma chamada GET ativada `me/devices`).</span><span class="sxs-lookup"><span data-stu-id="f1aa3-178">To use an app service you must do a POST call using the id of the device (obtained from doing a GET call on `me/devices`).</span></span> <span data-ttu-id="f1aa3-179">Para usar o exemplo a seguir, você deve instalar o [aplicativo Roma](https://aka.ms/romanapp) no seu dispositivo de destino.</span><span class="sxs-lookup"><span data-stu-id="f1aa3-179">To use the following example, you must install the [Rome app](https://aka.ms/romanapp) on your target device.</span></span>

<span data-ttu-id="f1aa3-180">Várias propriedades adicionais devem ser definidas na chamada.</span><span class="sxs-lookup"><span data-stu-id="f1aa3-180">Several additional properties must be set in the call.</span></span> <span data-ttu-id="f1aa3-181">O *tipo* deve ser definido *como serviço*, *AppServiceName* deve ser definido como o nome do serviço de aplicativo definido no aplicativo, *PackageFamilyName* deve ser definido como o nome da família do pacote definido no manifesto do aplicativo e *carga* contém as chaves e os valores para o serviço que você está chamando no aplicativo de destino.</span><span class="sxs-lookup"><span data-stu-id="f1aa3-181">*Type* must be set to *AppService*, *AppServiceName* must be set to the name of the app service defined in the application, *PackageFamilyName* must be set to the package family name defined in the app manifest, and *Payload* holds the keys and values for the service you are calling within the target application.</span></span>

#### <a name="request"></a><span data-ttu-id="f1aa3-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1aa3-182">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_command_2"
} -->

```http

POST me/devices/{id}/commands
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8

{
  "type" : "AppService",
  "appServiceName" : "com.microsoft.test.cdppingpongservice",
  "packageFamilyName" : "5085ShawnHenry.RomanTestApp_jsjw7knzsgcce",
  "payload" : {
    "Type":"Toast","Title":"Hello","Subtitle":"World!"}
  }
```

#### <a name="response"></a><span data-ttu-id="f1aa3-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1aa3-183">Response</span></span>

<span data-ttu-id="f1aa3-184">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f1aa3-184">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
  "isCollection": true
} -->

```http
HTTP/1.1 201 OK

{
  "id": "0158355AD4D680CC4E2994CC009EFFD7EADA8307E96FF1C8D19B..",
  "status": "requesting",
  "type": null,
  "appServiceName": "com.microsoft.randomnumbergenerator",
  "packageFamilyName": "Microsoft.SDKSamples.AppServicesProvider.CS_8wekyb3d8bbwe",
  "error": null,
  "permissionTicket": null,
  "postBackUri": null,
  "payload": {
    "Type": "Toast",
    "Title": "Hello",
    "Subtitle": "World!"
  }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/send-device-command.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
