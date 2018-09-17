# <a name="using-the-notifications-api-in-microsoft-graph-to-enable-human-centric-notification-experiences"></a>Usando a API de notificações no Microsoft Graph para habilitar experiências de notificação centradas em pessoas 

As notificações são a maneira mais eficaz de voltar a engajar seus usuários. Eles podem chamar a atenção dos usuários e trazê-los de volta para o seu aplicativo. Em um mundo multidispositivos, os usuários podem acessar seus aplicativos e serviços de qualquer lugar, em diferentes plataformas e dispositivos onde seus aplicativos estejam presentes. 

Seus cenários de notificação devem ser projetados com "foco em pessoas", com o principal objetivo de notificar o usuário, onde quer que ele ou ela esteja. As soluções de notificação existentes fornecidas pelas principais plataformas são excelentes para direcionamento de dispositivos. As notificações do Microsoft Graph tornam isso ainda melhor, permitindo que você defina usuários de destino. As notificações do Microsoft Graph farão todo o trabalho pesado, incluindo o mapeamento entre usuários e pontos de extremidade, a sincronização do estado de notificações pelos diferentes pontos de extremidade dos usuários, e muito mais. 

## <a name="why-integrate-with-microsoft-graph-notifications"></a>Por que integrar as notificações do Microsoft Graph?
### <a name="deliver-notifications-to-a-user-across-different-endpoints"></a>Entregue notificações para um usuário por diferentes pontos de extremidade
Como parte do Microsoft Graph, a API de notificações permite que você tenha como alvo uma conta da Microsoft, corporativa ou de estudante (do AD do Azure) para entregar uma notificação. A plataforma distribui essa notificação para todos os pontos de extremidade de todos os usuários, incluindo Windows UWP, Android e iOS. 

### <a name="manage-notifications-across-endpoints"></a>Gerenciar notificações entre pontos de extremidade
A API de notificações do Microsoft Graph permite que você atualize o estado de uma notificação de atualização e sincronize esse estado por todos os pontos de extremidade. Por exemplo, quando um usuário reage a uma notificação em um dispositivo, você pode atualizar o estado dessa notificação (por exemplo, marcá-la como lida ou ignorada), e essa mesma alteração de estado será distribuída para todos os outros pontos de extremidade. A API de notificações do Microsoft Graph rastreia o estado das notificações dos seus usuários de forma centralizada, tornando mais fácil de garantir que as notificações sejam manipuladas uma única vez e descartadas em todos os lugares.

### <a name="retrieve-notification-history"></a>Recuperar o histórico de notificações
Você pode usar a API de notificações para recuperar o histórico de notificações com base em uma data de expiração definida por você (até 30 dias). As notificações marcadas como lidas ou descartadas podem ser recuperadas do histórico, habilitando visualizações do histórico de notificações dentro do aplicativo e outros cenários. 

## <a name="integrating-with-the-notifications-api-in-microsoft-graph"></a>Integração com a API de notificações no Microsoft Graph

Você pode integrar seus aplicativos com as notificações do Microsoft Graph com algumas etapas simples - carregue o seu aplicativo por meio do Centro de Desenvolvimento do Windows, use o método de [Create notification](../api-reference/beta/api/projectrome_notification_post.md) para publicar notificações e use o SDK do Project Rome para receber e gerenciar notificações nos clientes do seu aplicativo.  

Para saber mais sobre como publicar notificações de usuário por meio do Microsoft Graph, consulte a [referência da API de notificações](../api-reference/beta/resources/notifications-api-overview.md).
 
Para saber mais sobre como receber e gerenciar notificações por meio da integração com o SDK do Project Rome, consulte a [documentação do SDK do Project Rome](https://docs.microsoft.com/en-us/windows/project-rome/) 

## <a name="see-also"></a>Confira também

- [Experiências entre dispositivos no Microsoft Graph](cross-device-concept-overview.md)
- [Centro de Desenvolvimento do Project Rome](http://aka.ms/projectrome)
