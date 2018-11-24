# <a name="microsoft-graph-security-api-error-responses"></a><span data-ttu-id="98058-101">Respostas de erros de API de segurança do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="98058-101">Microsoft Graph Security API error responses</span></span>

<span data-ttu-id="98058-102">Erros na API de segurança do Microsoft Graph no Microsoft Graph são retornados usando o código de status HTTP 206 parcial conteúdo padrão e são fornecidos por meio de um cabeçalho de aviso.</span><span class="sxs-lookup"><span data-stu-id="98058-102">Errors in the Microsoft Graph Security API in Microsoft Graph are returned using standard HTTP 206 Partial Content status code and are delivered by way of a warning header.</span></span>

<span data-ttu-id="98058-103">A API de segurança do Microsoft Graph é um serviço federado que recebe várias respostas de todos os provedores de dados.</span><span class="sxs-lookup"><span data-stu-id="98058-103">The Microsoft Graph Security API is a federated service that receives multiple responses from all data providers.</span></span> <span data-ttu-id="98058-104">Quando um erro HTTP é recebido pelo API de segurança do Microsoft Graph, ele retornará um cabeçalho de aviso no seguinte formato:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="98058-104">When an HTTP error is received by the Microsoft Graph Security API, it will send back a warning header in the following format: <!-- { "blockType": "ignored" } --></span></span>

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

<span data-ttu-id="98058-105">Este cabeçalho do aviso será enviado apenas para os clientes quando um dos provedores de dados retorna um código de erro que não seja 2xx ou 404.</span><span class="sxs-lookup"><span data-stu-id="98058-105">This warning header is only sent back to clients when one of the data providers returns an error code other than 2xx or 404.</span></span> <span data-ttu-id="98058-106">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="98058-106">For example:</span></span>

- <span data-ttu-id="98058-107">HttpStatusCode.Forbidden (403) pode ser retornado se o acesso ao recurso não é concedido.</span><span class="sxs-lookup"><span data-stu-id="98058-107">HttpStatusCode.Forbidden (403) might be returned if the access to the resource is not granted.</span></span>
- <span data-ttu-id="98058-108">Se um provedor de tempo limite, HttpStatusCode.GatewayTimeout (504) é retornado no cabeçalho do aviso.</span><span class="sxs-lookup"><span data-stu-id="98058-108">If a provider times out, HttpStatusCode.GatewayTimeout (504) is returned in the warning header.</span></span>
- <span data-ttu-id="98058-109">Se um erro interno do provedor acontecer, HttpStatusCode.InternalServerError (500) é usado no cabeçalho do aviso.</span><span class="sxs-lookup"><span data-stu-id="98058-109">If an internal provider error happens, HttpStatusCode.InternalServerError (500) is used in the warning header.</span></span>

<span data-ttu-id="98058-110">Se um provedor de dados retorna 2xx ou 404, ele não será mostrado no cabeçalho do aviso porque esses códigos esperados para o sucesso ou quando os dados não são encontrados respectivamente.</span><span class="sxs-lookup"><span data-stu-id="98058-110">If a data provider returns 2xx or 404, it’s not shown in the warning header because these codes are expected for success or when data is not found respectively.</span></span> <span data-ttu-id="98058-111">Em um sistema federado, um 404 não encontrado é esperado como muitas vezes, os dados somente são conhecidos por um ou vários, mas nem todos os provedores.</span><span class="sxs-lookup"><span data-stu-id="98058-111">In a federated system, a 404 not found is expected as many times the data is only known to one or several, but not all, providers.</span></span>

## <a name="example"></a><span data-ttu-id="98058-112">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98058-112">Example</span></span>

<span data-ttu-id="98058-113">Um usuário solicita `security/alerts/{alert_id}`.</span><span class="sxs-lookup"><span data-stu-id="98058-113">A user asks for `security/alerts/{alert_id}`.</span></span>

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

<span data-ttu-id="98058-114">Como 404 e 200 são condições esperadas, o cabeçalho do aviso contém o seguinte:</span><span class="sxs-lookup"><span data-stu-id="98058-114">Because both 404 and 200 are expected conditions, the warning header contains the following:</span></span> 

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> <span data-ttu-id="98058-115">**Observação:** Cada cabeçalho HTTP é uma coleção de subitems, para que os usuários possam enumerar o cabeçalho do aviso e verificar todos os itens.</span><span class="sxs-lookup"><span data-stu-id="98058-115">**Note:** Each HTTP header is a collection of subitems, so users can enumerate the Warning header and check all items.</span></span>

## <a name="see-also"></a><span data-ttu-id="98058-116">Confira também</span><span class="sxs-lookup"><span data-stu-id="98058-116">See also</span></span>

<span data-ttu-id="98058-117">Se você estiver tendo problemas com autorização, consulte nosso [postagem de blog](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2).</span><span class="sxs-lookup"><span data-stu-id="98058-117">If you’re having trouble with authorization, see our [blog post](https://techcommunity.microsoft.com/t5/Using-Microsoft-Graph-Security/Authorization-and-Microsoft-Graph-Security-API/m-p/184376#M2).</span></span>
