# <a name="security-api-error-responses"></a><span data-ttu-id="ac3fb-101">Respostas de erros da API de segurança</span><span class="sxs-lookup"><span data-stu-id="ac3fb-101">Security API error responses</span></span>

<span data-ttu-id="ac3fb-102">Erros da API de segurança do Microsoft Graph são retornados usando códigos de status padrão HTTP e são entregues como cabeçalho de aviso.</span><span class="sxs-lookup"><span data-stu-id="ac3fb-102">Errors in the security API in Microsoft Graph are returned using standard HTTP status codes and are delivered by way of a warning header.</span></span>

<span data-ttu-id="ac3fb-103">A API de segurança é um serviço federado que recebe várias respostas de todos os provedores de dados.</span><span class="sxs-lookup"><span data-stu-id="ac3fb-103">The security API is a federated service that receives multiple responses from all data providers.</span></span> <span data-ttu-id="ac3fb-104">Quando um erro HTTP é recebido pela API de segurança, ele retornará um cabeçalho de aviso no seguinte formato: <!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="ac3fb-104">When an HTTP error is received by the security API, it will send back a warning header in the following format: <!-- { "blockType": "ignored" } --></span></span>

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

<span data-ttu-id="ac3fb-105">Este cabeçalho de aviso será enviado de volta para os clientes somente quando um dos provedores de dados retornar um código de erro diferente de 2xx ou 404.</span><span class="sxs-lookup"><span data-stu-id="ac3fb-105">This warning header is only sent back to clients when one of the data providers returns an error code other than 2xx or 404.</span></span> <span data-ttu-id="ac3fb-106">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="ac3fb-106">For example:</span></span>

- <span data-ttu-id="ac3fb-107">HttpStatusCode.Forbidden (403) pode ser retornado se o acesso ao recurso não for concedido.</span><span class="sxs-lookup"><span data-stu-id="ac3fb-107">HttpStatusCode.Forbidden (403) might be returned if the access to the resource is not granted.</span></span>
- <span data-ttu-id="ac3fb-108">Se um provedor não responde a tempo, HttpStatusCode.GatewayTimeout (504) é retornado no cabeçalho de aviso.</span><span class="sxs-lookup"><span data-stu-id="ac3fb-108">If a provider times out, HttpStatusCode.GatewayTimeout (504) is returned in the warning header.</span></span>
- <span data-ttu-id="ac3fb-109">Se ocorrer um erro interno no provedor, HttpStatusCode.InternalServerError (500) é usado no cabeçalho de aviso.</span><span class="sxs-lookup"><span data-stu-id="ac3fb-109">If an internal provider error happens, HttpStatusCode.InternalServerError (500) is used in the warning header.</span></span>

<span data-ttu-id="ac3fb-110">Se um provedor de dados retornar 2xx ou 404, ele não será mostrado no cabeçalho do aviso porque esses são códigos esperados de êxito ou quando os dados não são encontrados, respectivamente.</span><span class="sxs-lookup"><span data-stu-id="ac3fb-110">If a data provider returns 2xx or 404, it’s not shown in the warning header because these codes are expected for success or when data is not found respectively.</span></span> <span data-ttu-id="ac3fb-111">Em um sistema federado, um erro 404 não encontrado é esperado, pois muitas vezes os dados são conhecidos por um ou vários provedores, mas não por todos.</span><span class="sxs-lookup"><span data-stu-id="ac3fb-111">In a federated system, a 404 not found is expected as many times the data is only known to one or several, but not all, providers.</span></span>

## <a name="example"></a><span data-ttu-id="ac3fb-112">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac3fb-112">Example</span></span>

<span data-ttu-id="ac3fb-113">Um usuário solicita `security/alerts/{alert_id}`.</span><span class="sxs-lookup"><span data-stu-id="ac3fb-113">A user asks for `security/alerts/{alert_id}`.</span></span>

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

<span data-ttu-id="ac3fb-114">Como 404 e 200 são condições esperadas, o cabeçalho do aviso contém o seguinte:</span><span class="sxs-lookup"><span data-stu-id="ac3fb-114">Because both 404 and 200 are expected conditions, the warning header contains the following:</span></span> 

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/29000",    (usual timeout limit is set at 29 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> <span data-ttu-id="ac3fb-115">**Observação:** Cada cabeçalho HTTP é uma coleção de subitems, para que os usuários possam enumerar o cabeçalho de aviso e verificar todos os itens.</span><span class="sxs-lookup"><span data-stu-id="ac3fb-115">**Note:** Each HTTP header is a collection of subitems, so users can enumerate the Warning header and check all items.</span></span>

## <a name="see-also"></a><span data-ttu-id="ac3fb-116">Confira também</span><span class="sxs-lookup"><span data-stu-id="ac3fb-116">See also</span></span>

<span data-ttu-id="ac3fb-117">Se você estiver tendo problemas com autorização, confira nossa [postagem no blog](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2).</span><span class="sxs-lookup"><span data-stu-id="ac3fb-117">If you’re having trouble with authorization, see our [blog post](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2).</span></span>
