@id("LimitDeveloperCreateAccess")
permit (
  principal in Jans::Role::"developer",
  action in [Jans::Action::"Create"],
  resource is Jans::VirtualMachine
)
when {
  principal has id_token.limit &&
  principal.id_token.limit > 0
};